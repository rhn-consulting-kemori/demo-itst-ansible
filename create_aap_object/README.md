# Create Ansible Automation Contoroller Object
## Project
* demo-itst-project
* Git
* https://github.com/rhn-consulting-kemori/demo-itst-ansible.git
## Credentials
* ocp_credential
### type
* OpenShift or Kubernetes API Bearer Token
### endpoint
* sample -> https://api.rosa-nsdsm.9et7.p3.openshiftapps.com
### Token
* OpenShift-CLIの以下コマンドで取得したトークンを設定
* oc whoami --show-token
### SSL認証
* しない
## Inventory
* demo-itst-inventory
### Reference
* inventory/inventory_all_vars.yaml
## Create JobTemplate
* create_app_object/create_jobtemplate.yaml
## Create WorkflowJob
* create_app_object/create_workflow.yaml