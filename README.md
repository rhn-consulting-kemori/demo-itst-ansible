# demo-itst-ansible
## OpenShift Credential
### Get OpenShift Token Command
* oc whoami --show-token
### Set Credential
* Ansibleで認証情報を選択して追加をクリック
* 名前を入力して認証タイプを「OpenShift または Kubernetes API Bearerトークン」にし、OpenShiftまたは Kubernetes APIエンドポイント と API認証ベアラートークン を入力
* 今回はSSLの検証はしないのでチェックを外して保存
## Ansible
### Ansible Token
* User > UserName > Tokens
* Create token
* Personal access token
## Inventory
* inventory/inventory_all_vars.yaml
## Ansible API URL
### AAP2.5
* {{ aap_controller_url }}/api/controller/v2/workflow_job_templates/{{ environment_pipeline_number }}/launch/
### AAP2.4 Before
* {{ aap_controller_url }}/api/v2/workflow_job_templates/{{ environment_pipeline_number }}/launch/
