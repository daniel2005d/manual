# Comandos de az cli
> Descarga https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-apt?view=azure-cli-latest

* az [comando] --help : Ayuda del comando
* az login : Autenticacion
* az account set --subscription [nombre]: Establece la cuenta o suscripcion por defecto
* az account list-locations: Muestra permisos y zonas
* az group create --name "[nombre del grupo]" --location "[ubicación]" : Crea un grupo de recursos

### Maquina Virtual
1. Red Virtual
* az network vnet create --resource-group "nombre" --name "name" --address-prefix "name" --subnet-prefix "xxx.xxx.xxx.0/mask"
2. IP Publica
* az network public-ip create --resource-group "nombre" --name "name"
3. Grupo de Seguridad
* az network nsg create  => Incompleto
4. Interfaz de red
* az network nic create --resource-group "" -- name "" --vnet-name "" => Incompleto
5. Maquina virtual
* az vm create --resource-group "" --location "" --name "" --nics "" --image "" --admin-username "" --authentication-type "" --ssh-key-value ""

az vm open-port : Abrir puerto
az vm list-ip-addresses --name "" : Direccion IP de la maquina
* az group delete --name "" --no-wait: Eliminacion del grupo de recursos
** --no-wait: No bloquea la consola
* az vm show --name "" --resource-group "" --output table : Muestra el detalle de ubicación de la VM.
** --output: Formato de Salida 

## Cuentas de Almacenamiento

* az storage account create --kind StorageV2 --resource-group "" --location "" --name ""
* az storage blob upload --file "" --container-name "" --name "filename" --account-name ""
