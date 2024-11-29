# for CNDW 2024 dem


Base: Contains the generic yaml files that will provide the basis for the building of our virtual machines.

    - *base-vm.yaml* contains the basic specifications for our virtual machine configuration.

Overlays: Contains the subdirectories "dev" and "prod" which provide the customizations for a hypothetical development and production environment. 

    - *kustomization.yaml* which defines the resources to be used.

Dev and Prod subdirectories: Each contains files to be used to customize environments. 

    - *config.yaml* is used to change the names of resources based on the virtual machine names.
    - **-vm-patch.yaml* files contain some simple patches to modify the specs of the VMs. It also sets running=true so the machine start up after creation.

