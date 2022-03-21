## The Provider can be used to create and destroy a github repo.
'resource "github_repository" "example" {
  name        = "example"
  description = "My awesome codebase"

  visibility = "public"
	auto_init  = "true"
}'
## Furthermore we can use a template option in the github_repository resource to create a Repository from a template.
' template {
    owner      = "github"
    repository = "terraform-module-template"
  }'

