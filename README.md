# evocloud-oci
Repository with OCI resources: Helm Charts and Container Images

## 🚀 Pushing Docker Images
Here is an example workflow on how to push OCI compliant docker images into the evocloud-oci repository:

### 🤖 Login to ghcr.io using your Personal Access Token
``docker login ghcr.io -u myUsername`` (You will be prompted to enter your Personal Access Token

### 🪝 Pull, Tag, and Push an Image
```
docker pull alpine/terragrunt:1.11.3
docker image tag ac9ba070d625d1977a696c3e639e5afa02618094854bf4f033f6ea832ed4a5ab ghcr.io/evocloud-dev/evocloud-oci/alpine/terragrunt:1.11.3
docker push ghcr.io/evocloud-dev/evocloud-oci/alpine/terragrunt:1.11.3
```
### ✅ Verify 
To verify the pushed image made it to the right repository go to https://github.com/evocloud-dev > and select Packages.

