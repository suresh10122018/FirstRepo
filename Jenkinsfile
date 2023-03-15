node{
    stage 'Checkout Terraform Project'
        git 'https://github.com/suresh10122018/terraformrepo.git'
    stage 'INIT'
        bat 'terraform init'
    stage 'SANITY CHECK'
        bat 'terraform validate'
    stage 'PLAN'
        bat 'terraform plan -out "s3.tfplan"'
    stage 'FORMAT'
        bat 'terraform fmt'
    stage 'APPLY'
        bat 'terraform apply "s3.tfplan"'    
}
