# Comparing `tmp/solutions_builder-1.18.0.tar.gz` & `tmp/solutions_builder-1.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_builder-1.18.0.tar", max compression
+gzip compressed data, was "solutions_builder-1.18.1.tar", max compression
```

## Comparing `solutions_builder-1.18.0.tar` & `solutions_builder-1.18.1.tar`

### file list

```diff
@@ -1,237 +1,238 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.18.0/LICENSE
--rw-r--r--   0        0        0     5636 2024-04-14 21:46:23.164280 solutions_builder-1.18.0/README.md
--rw-r--r--   0        0        0     1148 2024-04-14 20:49:54.057476 solutions_builder-1.18.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.724132 solutions_builder-1.18.0/solutions_builder/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.730627 solutions_builder-1.18.0/solutions_builder/cli/__init__.py
--rw-r--r--   0        0        0    10056 2024-04-14 21:44:15.880745 solutions_builder-1.18.0/solutions_builder/cli/cli.py
--rw-r--r--   0        0        0      773 2024-03-25 03:04:07.741379 solutions_builder-1.18.0/solutions_builder/cli/cli_constants.py
--rw-r--r--   0        0        0     4810 2024-03-25 03:04:07.748052 solutions_builder-1.18.0/solutions_builder/cli/cli_utils.py
--rw-r--r--   0        0        0     7362 2024-04-14 21:37:17.430667 solutions_builder-1.18.0/solutions_builder/cli/component.py
--rw-r--r--   0        0        0     6347 2024-04-14 21:02:16.843261 solutions_builder-1.18.0/solutions_builder/cli/infra.py
--rw-r--r--   0        0        0     2567 2024-04-14 21:02:48.815027 solutions_builder-1.18.0/solutions_builder/cli/set.py
--rw-r--r--   0        0        0     1429 2024-04-14 21:03:11.981839 solutions_builder-1.18.0/solutions_builder/cli/template.py
--rw-r--r--   0        0        0     5828 2024-04-14 21:03:17.359957 solutions_builder-1.18.0/solutions_builder/cli/vars.py
--rw-r--r--   0        0        0     3942 2024-03-25 03:04:07.751131 solutions_builder-1.18.0/solutions_builder/cli/vars_test.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.752671 solutions_builder-1.18.0/solutions_builder/copier_extensions/__init__.py
--rw-r--r--   0        0        0     1563 2024-03-25 03:04:07.756910 solutions_builder-1.18.0/solutions_builder/copier_extensions/context.py
--rw-r--r--   0        0        0     6126 2024-03-25 03:04:07.757820 solutions_builder-1.18.0/solutions_builder/copier_extensions/sb_helpers.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.760026 solutions_builder-1.18.0/solutions_builder/fragments/skaffold_template/copier.yaml
--rw-r--r--   0        0        0      101 2024-03-25 03:04:07.760859 solutions_builder-1.18.0/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
--rw-r--r--   0        0        0      766 2024-03-25 03:04:07.761736 solutions_builder-1.18.0/solutions_builder/module_template/README.md
--rw-r--r--   0        0        0      865 2024-03-25 03:04:07.762000 solutions_builder-1.18.0/solutions_builder/module_template/copier.yaml
--rw-r--r--   0        0        0       89 2024-03-25 03:04:07.762719 solutions_builder-1.18.0/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
--rw-r--r--   0        0        0     1135 2024-03-25 03:04:07.763039 solutions_builder-1.18.0/solutions_builder/module_template/template_copier.yaml
--rw-r--r--   0        0        0     3878 2024-03-25 03:04:07.765629 solutions_builder-1.18.0/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
--rw-r--r--   0        0        0      566 2024-03-25 03:04:07.767359 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
--rw-r--r--   0        0        0      109 2024-03-25 03:04:07.767845 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
--rw-r--r--   0        0        0     3204 2024-03-25 03:04:07.768208 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
--rw-r--r--   0        0        0      590 2024-03-25 03:04:07.768754 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
--rw-r--r--   0        0        0       81 2024-03-25 03:04:07.769062 solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
--rw-r--r--   0        0        0      736 2024-03-25 03:04:07.771134 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
--rw-r--r--   0        0        0      636 2024-03-25 03:04:07.771582 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
--rw-r--r--   0        0        0      836 2024-03-25 03:04:07.772094 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
--rw-r--r--   0        0        0      777 2024-03-25 03:04:07.772440 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
--rw-r--r--   0        0        0      858 2024-03-25 03:04:07.772726 solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.775721 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0      545 2024-03-25 03:04:07.777691 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1300 2024-03-25 03:04:07.778047 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/README.md
--rw-r--r--   0        0        0       77 2024-03-25 03:04:07.778421 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0       98 2024-03-25 03:04:07.778741 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     2974 2024-03-25 03:04:07.779722 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0     1610 2024-04-14 20:43:56.364650 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0      903 2024-03-25 03:04:07.780746 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/routes/sample.py
--rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.781845 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2024-03-25 03:04:07.782124 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2024-03-25 03:04:07.783108 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2024-03-25 03:04:07.783376 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2024-03-25 03:04:07.783937 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2024-03-25 03:04:07.784849 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0      215 2024-03-25 03:04:07.785391 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'manifests' if deploy_cloudrun else ''}}/cloudrun-service.yaml
--rw-r--r--   0        0        0       92 2024-03-25 03:04:07.785799 solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/skaffold.yaml.patch
--rw-r--r--   0        0        0     2095 2024-03-25 03:04:07.786572 solutions_builder-1.18.0/solutions_builder/modules/blank_service/copier.yaml
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.787312 solutions_builder-1.18.0/solutions_builder/modules/restful_service/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1363 2024-03-25 03:04:07.787571 solutions_builder-1.18.0/solutions_builder/modules/restful_service/README.md
--rw-r--r--   0        0        0      545 2024-03-25 03:04:07.788965 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1309 2024-03-25 03:04:07.789227 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0       77 2024-03-25 03:04:07.789564 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0       98 2024-03-25 03:04:07.789873 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     2974 2024-03-25 03:04:07.790203 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      862 2024-03-25 03:04:07.791788 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1711 2024-03-25 03:04:07.792135 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1725 2024-04-14 20:43:56.364892 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.793877 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3876 2024-03-25 03:04:07.796299 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0     1222 2024-03-25 03:04:07.796775 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.797162 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.797870 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2024-03-25 03:04:07.798184 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2024-03-25 03:04:07.798460 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2024-03-25 03:04:07.798769 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2024-03-25 03:04:07.799347 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2024-03-25 03:04:07.799631 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0      215 2024-03-25 03:04:07.800125 solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'manifests' if deploy_cloudrun else ''}}/cloudrun-service.yaml
--rw-r--r--   0        0        0     2305 2024-03-25 03:04:07.803460 solutions_builder-1.18.0/solutions_builder/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0      120 2024-03-25 03:04:07.804550 solutions_builder-1.18.0/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2024-03-25 03:04:07.804816 solutions_builder-1.18.0/solutions_builder/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2024-03-25 03:04:07.806500 solutions_builder-1.18.0/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3223 2024-03-25 03:04:07.808817 solutions_builder-1.18.0/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2024-03-25 03:04:07.809387 solutions_builder-1.18.0/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.811569 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1572 2024-03-25 03:04:07.811814 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/README.md
--rw-r--r--   0        0        0      545 2024-03-25 03:04:07.813321 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0      215 2024-03-25 03:04:07.813936 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2024-03-25 03:04:07.814203 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      143 2024-03-25 03:04:07.814453 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3193 2024-03-25 03:04:07.814770 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      942 2024-03-25 03:04:07.816878 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1751 2024-03-25 03:04:07.817133 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1550 2024-03-25 03:04:07.818717 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.819395 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     5195 2024-03-25 03:04:07.822303 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
--rw-r--r--   0        0        0     1196 2024-03-25 03:04:07.823423 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.823723 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.824495 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
--rw-r--r--   0        0        0      430 2024-03-25 03:04:07.825744 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
--rw-r--r--   0        0        0     1348 2024-03-25 03:04:07.827789 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
--rw-r--r--   0        0        0     1138 2024-03-25 03:04:07.828088 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
--rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.828856 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2024-03-25 03:04:07.829109 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       97 2024-03-25 03:04:07.829359 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2024-03-25 03:04:07.829594 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2024-03-25 03:04:07.829956 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2024-03-25 03:04:07.830168 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2667 2024-03-25 03:04:07.830370 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/copier.yaml
--rw-r--r--   0        0        0       71 2024-03-25 03:04:07.830981 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2024-03-25 03:04:07.831165 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      719 2024-03-25 03:04:07.833442 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
--rw-r--r--   0        0        0     2693 2024-03-25 03:04:07.833738 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
--rw-r--r--   0        0        0      930 2024-03-25 03:04:07.834108 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
--rw-r--r--   0        0        0     1320 2024-03-25 03:04:07.834369 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
--rw-r--r--   0        0        0     2076 2024-03-25 03:04:07.834641 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
--rw-r--r--   0        0        0     3851 2024-03-25 03:04:07.835330 solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.836211 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1374 2024-03-25 03:04:07.836431 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      784 2024-03-25 03:04:07.837033 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0      763 2024-03-25 03:04:07.837791 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/backend.tf
--rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.838178 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/iam.tf
--rw-r--r--   0        0        0     2486 2024-03-25 03:04:07.838410 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/main.tf
--rw-r--r--   0        0        0     1783 2024-03-25 03:04:07.838671 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/providers.tf
--rw-r--r--   0        0        0      308 2024-03-25 03:04:07.838982 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
--rw-r--r--   0        0        0     1553 2024-03-25 03:04:07.839201 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/variables.tf
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.839951 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0      946 2024-03-25 03:04:07.840151 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/copier.yaml
--rw-r--r--   0        0        0      650 2024-03-25 03:04:07.840804 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0      763 2024-03-25 03:04:07.841462 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/backend.tf
--rw-r--r--   0        0        0     1490 2024-03-25 03:04:07.841826 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/main.tf
--rw-r--r--   0        0        0     1002 2024-03-25 03:04:07.842816 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/providers.tf
--rw-r--r--   0        0        0      138 2024-03-25 03:04:07.843058 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
--rw-r--r--   0        0        0     1140 2024-03-25 03:04:07.843413 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/variables.tf
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.845118 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     2396 2024-03-25 03:04:07.845466 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/copier.yaml
--rw-r--r--   0        0        0      181 2024-03-25 03:04:07.846354 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
--rw-r--r--   0        0        0      658 2024-03-25 03:04:07.846642 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
--rw-r--r--   0        0        0      145 2024-03-25 03:04:07.846979 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
--rw-r--r--   0        0        0      225 2024-03-25 03:04:07.847261 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
--rw-r--r--   0        0        0      378 2024-03-25 03:04:07.852866 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
--rw-r--r--   0        0        0       59 2024-03-25 03:04:07.853875 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
--rw-r--r--   0        0        0     1695 2024-03-25 03:04:07.858750 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2024-03-25 03:04:07.859082 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1264 2024-03-25 03:04:07.860615 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0      752 2024-04-14 20:43:56.365155 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/backend.tf
--rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.861621 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/iam.tf
--rw-r--r--   0        0        0     1695 2024-03-25 03:04:07.861857 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/main.tf
--rw-r--r--   0        0        0     1877 2024-03-25 03:04:07.862898 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/providers.tf
--rw-r--r--   0        0        0      520 2024-03-25 03:04:07.863221 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
--rw-r--r--   0        0        0     1802 2024-03-25 03:04:07.863461 solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/variables.tf
--rw-r--r--   0        0        0       80 2024-03-25 03:04:07.864843 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/.sb/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1048 2024-03-25 03:04:07.865072 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      877 2024-04-14 20:43:56.365414 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2024-03-25 03:04:07.866341 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      670 2024-03-25 03:04:07.866546 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2024-03-25 03:04:07.866888 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2024-03-25 03:04:07.867470 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      236 2024-03-25 03:04:07.867794 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1984 2024-03-25 03:04:07.868153 solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       90 2024-03-25 03:04:07.868658 solutions_builder-1.18.0/solutions_builder/requirements.txt
--rw-r--r--   0        0        0    68957 2024-03-25 03:04:07.870229 solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2024-03-25 03:04:07.870988 solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2637 2024-03-25 03:04:07.871475 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2688 2024-03-25 03:04:07.871683 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5784 2024-03-25 03:04:07.872126 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8047 2024-03-25 03:04:07.874328 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3129 2024-03-25 03:04:07.874720 solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2024-03-25 03:04:07.875041 solutions_builder-1.18.0/solutions_builder/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2024-03-25 03:04:07.876082 solutions_builder-1.18.0/solutions_builder/template_root/.pylintrc
--rw-r--r--   0        0        0     4878 2024-03-25 03:04:07.876530 solutions_builder-1.18.0/solutions_builder/template_root/README.md
--rw-r--r--   0        0        0      398 2024-03-25 03:04:07.876998 solutions_builder-1.18.0/solutions_builder/template_root/components/README.md
--rw-r--r--   0        0        0      893 2024-03-25 03:04:07.877867 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
--rw-r--r--   0        0        0     1101 2024-03-25 03:04:07.878112 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
--rw-r--r--   0        0        0      111 2024-03-25 03:04:07.878424 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
--rw-r--r--   0        0        0      240 2024-03-25 03:04:07.878829 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
--rw-r--r--   0        0        0      571 2024-03-25 03:04:07.879408 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.880848 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
--rw-r--r--   0        0        0      831 2024-03-25 03:04:07.881462 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
--rw-r--r--   0        0        0      695 2024-03-25 03:04:07.881658 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
--rw-r--r--   0        0        0       35 2024-03-25 03:04:07.882687 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
--rw-r--r--   0        0        0       91 2024-03-25 03:04:07.882932 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
--rw-r--r--   0        0        0     1376 2024-03-25 03:04:07.884644 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.885395 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
--rw-r--r--   0        0        0      754 2024-03-25 03:04:07.887849 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1006 2024-03-25 03:04:07.888076 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2243 2024-03-25 03:04:07.888314 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.889468 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1002 2024-03-25 03:04:07.891212 solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2500 2024-03-25 03:04:07.891459 solutions_builder-1.18.0/solutions_builder/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2024-03-25 03:04:07.891699 solutions_builder-1.18.0/solutions_builder/template_root/firebase.json
--rw-r--r--   0        0        0      484 2024-04-14 21:44:49.817394 solutions_builder-1.18.0/solutions_builder/template_root/sb.yaml
--rw-r--r--   0        0        0       98 2024-03-25 03:04:07.892621 solutions_builder-1.18.0/solutions_builder/template_root/setup.cfg
--rw-r--r--   0        0        0      215 2024-03-25 03:04:07.893127 solutions_builder-1.18.0/solutions_builder/template_root/skaffold.yaml
--rw-r--r--   0        0        0      921 2024-03-25 03:04:07.894470 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2024-03-25 03:04:07.894809 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2024-03-25 03:04:07.895330 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2024-03-25 03:04:07.895611 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2024-03-25 03:04:07.896165 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2024-03-25 03:04:07.896402 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1186 2024-03-25 03:04:07.896659 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2024-03-25 03:04:07.896925 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2024-03-25 03:04:07.897379 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2024-03-25 03:04:07.897631 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     3868 2024-03-25 03:04:07.898055 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2024-03-25 03:04:07.898338 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     3453 2024-03-25 03:04:07.898588 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     3012 2024-03-25 03:04:07.899082 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2024-03-25 03:04:07.899396 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2024-03-25 03:04:07.899720 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2024-03-25 03:04:07.900599 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      774 2024-03-25 03:04:07.900949 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2024-03-25 03:04:07.901558 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2024-03-25 03:04:07.902536 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2024-03-25 03:04:07.905914 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      678 2024-03-25 03:04:07.906314 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2024-03-25 03:04:07.906938 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2024-03-25 03:04:07.907328 solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2561 2024-03-25 03:04:07.908063 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/bastion_startup.sh
--rw-r--r--   0        0        0     3593 2024-03-25 03:04:07.909125 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/main.tf
--rw-r--r--   0        0        0      178 2024-03-25 03:04:07.909456 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/terraform.tfvars
--rw-r--r--   0        0        0      782 2024-03-25 03:04:07.910038 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/variables.tf
--rw-r--r--   0        0        0     2873 2024-03-25 03:04:07.910583 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2024-03-25 03:04:07.910858 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       86 2024-03-25 03:04:07.911144 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2024-03-25 03:04:07.911400 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      869 2024-04-14 20:43:56.365662 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0     1669 2024-03-25 03:04:07.912198 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.912485 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0     1032 2024-03-25 03:04:07.912743 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf
--rw-r--r--   0        0        0     4602 2024-03-25 03:04:07.913103 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      991 2024-03-25 03:04:07.913405 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      921 2024-03-25 03:04:07.913735 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      724 2024-03-25 03:04:07.914076 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2839 2024-03-25 03:04:07.914408 solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.914895 solutions_builder-1.18.0/solutions_builder/template_root/tests/__init__.py
--rw-r--r--   0        0        0     1386 2024-03-25 03:04:07.915482 solutions_builder-1.18.0/solutions_builder/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      952 2024-03-25 03:04:07.915993 solutions_builder-1.18.0/solutions_builder/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0      990 2024-03-25 03:04:07.916378 solutions_builder-1.18.0/solutions_builder/template_root/utils/init_env_vars.sh
--rwxr-xr-x   0        0        0     1845 2024-03-25 03:04:07.917312 solutions_builder-1.18.0/solutions_builder/template_root/utils/setup_ksa.sh
--rw-r--r--   0        0        0       81 2024-03-25 03:04:07.917579 solutions_builder-1.18.0/solutions_builder/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2024-03-25 03:04:07.917901 solutions_builder-1.18.0/solutions_builder/tests/__init__.py
--rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 solutions_builder-1.18.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.18.1/LICENSE
+-rw-r--r--   0        0        0     5636 2024-04-29 01:47:30.406912 solutions_builder-1.18.1/README.md
+-rw-r--r--   0        0        0     1148 2024-04-29 02:04:00.644545 solutions_builder-1.18.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.724132 solutions_builder-1.18.1/solutions_builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.730627 solutions_builder-1.18.1/solutions_builder/cli/__init__.py
+-rw-r--r--   0        0        0    10056 2024-04-29 01:47:30.409005 solutions_builder-1.18.1/solutions_builder/cli/cli.py
+-rw-r--r--   0        0        0      773 2024-03-25 03:04:07.741379 solutions_builder-1.18.1/solutions_builder/cli/cli_constants.py
+-rw-r--r--   0        0        0     4810 2024-03-25 03:04:07.748052 solutions_builder-1.18.1/solutions_builder/cli/cli_utils.py
+-rw-r--r--   0        0        0     7362 2024-04-29 01:47:30.409352 solutions_builder-1.18.1/solutions_builder/cli/component.py
+-rw-r--r--   0        0        0     6347 2024-04-29 01:47:30.409685 solutions_builder-1.18.1/solutions_builder/cli/infra.py
+-rw-r--r--   0        0        0     2567 2024-04-29 01:47:30.409965 solutions_builder-1.18.1/solutions_builder/cli/set.py
+-rw-r--r--   0        0        0     1429 2024-04-29 01:47:30.410154 solutions_builder-1.18.1/solutions_builder/cli/template.py
+-rw-r--r--   0        0        0     5828 2024-04-29 01:47:30.410419 solutions_builder-1.18.1/solutions_builder/cli/vars.py
+-rw-r--r--   0        0        0     3942 2024-03-25 03:04:07.751131 solutions_builder-1.18.1/solutions_builder/cli/vars_test.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.752671 solutions_builder-1.18.1/solutions_builder/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     1563 2024-03-25 03:04:07.756910 solutions_builder-1.18.1/solutions_builder/copier_extensions/context.py
+-rw-r--r--   0        0        0     6126 2024-03-25 03:04:07.757820 solutions_builder-1.18.1/solutions_builder/copier_extensions/sb_helpers.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.760026 solutions_builder-1.18.1/solutions_builder/fragments/skaffold_template/copier.yaml
+-rw-r--r--   0        0        0      101 2024-03-25 03:04:07.760859 solutions_builder-1.18.1/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
+-rw-r--r--   0        0        0      766 2024-03-25 03:04:07.761736 solutions_builder-1.18.1/solutions_builder/module_template/README.md
+-rw-r--r--   0        0        0      865 2024-03-25 03:04:07.762000 solutions_builder-1.18.1/solutions_builder/module_template/copier.yaml
+-rw-r--r--   0        0        0       89 2024-03-25 03:04:07.762719 solutions_builder-1.18.1/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
+-rw-r--r--   0        0        0     1135 2024-03-25 03:04:07.763039 solutions_builder-1.18.1/solutions_builder/module_template/template_copier.yaml
+-rw-r--r--   0        0        0     3878 2024-03-25 03:04:07.765629 solutions_builder-1.18.1/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
+-rw-r--r--   0        0        0      566 2024-03-25 03:04:07.767359 solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
+-rw-r--r--   0        0        0      109 2024-03-25 03:04:07.767845 solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
+-rw-r--r--   0        0        0     3204 2024-03-25 03:04:07.768208 solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
+-rw-r--r--   0        0        0      590 2024-03-25 03:04:07.768754 solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
+-rw-r--r--   0        0        0       81 2024-03-25 03:04:07.769062 solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
+-rw-r--r--   0        0        0      736 2024-03-25 03:04:07.771134 solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
+-rw-r--r--   0        0        0      636 2024-03-25 03:04:07.771582 solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
+-rw-r--r--   0        0        0      836 2024-03-25 03:04:07.772094 solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
+-rw-r--r--   0        0        0      777 2024-03-25 03:04:07.772440 solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
+-rw-r--r--   0        0        0      858 2024-03-25 03:04:07.772726 solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.775721 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0      545 2024-03-25 03:04:07.777691 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1300 2024-03-25 03:04:07.778047 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0       77 2024-03-25 03:04:07.778421 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2024-03-25 03:04:07.778741 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2024-03-25 03:04:07.779722 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      911 2024-04-29 01:47:52.546593 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1610 2024-04-29 01:47:30.410746 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0      903 2024-04-29 01:47:30.411096 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/routes/sample.py
+-rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.781845 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2024-03-25 03:04:07.782124 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2024-03-25 03:04:07.783108 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2024-03-25 03:04:07.783376 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2024-03-25 03:04:07.783937 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2024-03-25 03:04:07.784849 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.785391 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'manifests' if deploy_cloudrun else ''}}/cloudrun-service.yaml
+-rw-r--r--   0        0        0       92 2024-03-25 03:04:07.785799 solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/skaffold.yaml.patch
+-rw-r--r--   0        0        0     2095 2024-03-25 03:04:07.786572 solutions_builder-1.18.1/solutions_builder/modules/blank_service/copier.yaml
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.787312 solutions_builder-1.18.1/solutions_builder/modules/restful_service/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1363 2024-03-25 03:04:07.787571 solutions_builder-1.18.1/solutions_builder/modules/restful_service/README.md
+-rw-r--r--   0        0        0      545 2024-03-25 03:04:07.788965 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1309 2024-03-25 03:04:07.789227 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0       77 2024-03-25 03:04:07.789564 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2024-03-25 03:04:07.789873 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2024-03-25 03:04:07.790203 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      862 2024-03-25 03:04:07.791788 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1711 2024-03-25 03:04:07.792135 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1725 2024-04-29 01:47:30.411393 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.793877 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2024-03-25 03:04:07.796299 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2024-03-25 03:04:07.796775 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.797162 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.797870 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2024-03-25 03:04:07.798184 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2024-03-25 03:04:07.798460 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2024-03-25 03:04:07.798769 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2024-03-25 03:04:07.799347 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2024-03-25 03:04:07.799631 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.800125 solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'manifests' if deploy_cloudrun else ''}}/cloudrun-service.yaml
+-rw-r--r--   0        0        0     2305 2024-03-25 03:04:07.803460 solutions_builder-1.18.1/solutions_builder/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0      120 2024-03-25 03:04:07.804550 solutions_builder-1.18.1/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2024-03-25 03:04:07.804816 solutions_builder-1.18.1/solutions_builder/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2024-03-25 03:04:07.806500 solutions_builder-1.18.1/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3223 2024-03-25 03:04:07.808817 solutions_builder-1.18.1/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2024-03-25 03:04:07.809387 solutions_builder-1.18.1/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.811569 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1572 2024-03-25 03:04:07.811814 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/README.md
+-rw-r--r--   0        0        0      545 2024-03-25 03:04:07.813321 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.813936 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2024-03-25 03:04:07.814203 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      143 2024-03-25 03:04:07.814453 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3193 2024-03-25 03:04:07.814770 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      942 2024-03-25 03:04:07.816878 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1751 2024-03-25 03:04:07.817133 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1550 2024-03-25 03:04:07.818717 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.819395 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     5195 2024-03-25 03:04:07.822303 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
+-rw-r--r--   0        0        0     1196 2024-03-25 03:04:07.823423 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.823723 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.824495 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
+-rw-r--r--   0        0        0      430 2024-03-25 03:04:07.825744 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
+-rw-r--r--   0        0        0     1348 2024-03-25 03:04:07.827789 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
+-rw-r--r--   0        0        0     1138 2024-03-25 03:04:07.828088 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
+-rw-r--r--   0        0        0     1232 2024-03-25 03:04:07.828856 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2024-03-25 03:04:07.829109 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       97 2024-03-25 03:04:07.829359 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2024-03-25 03:04:07.829594 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2024-03-25 03:04:07.829956 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2024-03-25 03:04:07.830168 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2667 2024-03-25 03:04:07.830370 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/copier.yaml
+-rw-r--r--   0        0        0       71 2024-03-25 03:04:07.830981 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2024-03-25 03:04:07.831165 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      719 2024-03-25 03:04:07.833442 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
+-rw-r--r--   0        0        0     2693 2024-03-25 03:04:07.833738 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
+-rw-r--r--   0        0        0      930 2024-03-25 03:04:07.834108 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
+-rw-r--r--   0        0        0     1320 2024-03-25 03:04:07.834369 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
+-rw-r--r--   0        0        0     2076 2024-03-25 03:04:07.834641 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
+-rw-r--r--   0        0        0     3851 2024-03-25 03:04:07.835330 solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.836211 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1374 2024-03-25 03:04:07.836431 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      784 2024-03-25 03:04:07.837033 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0      763 2024-03-25 03:04:07.837791 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/backend.tf
+-rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.838178 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/iam.tf
+-rw-r--r--   0        0        0     2486 2024-03-25 03:04:07.838410 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/main.tf
+-rw-r--r--   0        0        0     1783 2024-03-25 03:04:07.838671 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/providers.tf
+-rw-r--r--   0        0        0      308 2024-03-25 03:04:07.838982 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
+-rw-r--r--   0        0        0     1553 2024-03-25 03:04:07.839201 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.839951 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0      946 2024-03-25 03:04:07.840151 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/copier.yaml
+-rw-r--r--   0        0        0      650 2024-03-25 03:04:07.840804 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0      763 2024-03-25 03:04:07.841462 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/backend.tf
+-rw-r--r--   0        0        0     1490 2024-03-25 03:04:07.841826 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/main.tf
+-rw-r--r--   0        0        0     1002 2024-03-25 03:04:07.842816 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/providers.tf
+-rw-r--r--   0        0        0      138 2024-03-25 03:04:07.843058 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
+-rw-r--r--   0        0        0     1140 2024-03-25 03:04:07.843413 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-03-25 03:04:07.845118 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     2396 2024-03-25 03:04:07.845466 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/copier.yaml
+-rw-r--r--   0        0        0      181 2024-03-25 03:04:07.846354 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
+-rw-r--r--   0        0        0      658 2024-03-25 03:04:07.846642 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
+-rw-r--r--   0        0        0      145 2024-03-25 03:04:07.846979 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
+-rw-r--r--   0        0        0      225 2024-03-25 03:04:07.847261 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
+-rw-r--r--   0        0        0      378 2024-03-25 03:04:07.852866 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
+-rw-r--r--   0        0        0       59 2024-03-25 03:04:07.853875 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
+-rw-r--r--   0        0        0     1695 2024-03-25 03:04:07.858750 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2024-03-25 03:04:07.859082 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1264 2024-03-25 03:04:07.860615 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0      752 2024-04-29 01:47:30.411670 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/backend.tf
+-rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.861621 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/iam.tf
+-rw-r--r--   0        0        0     1695 2024-03-25 03:04:07.861857 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/main.tf
+-rw-r--r--   0        0        0     1877 2024-03-25 03:04:07.862898 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/providers.tf
+-rw-r--r--   0        0        0      520 2024-03-25 03:04:07.863221 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/terraform.tfvars
+-rw-r--r--   0        0        0     1802 2024-03-25 03:04:07.863461 solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/variables.tf
+-rw-r--r--   0        0        0       80 2024-04-29 01:47:30.412385 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1048 2024-03-25 03:04:07.865072 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      877 2024-04-29 01:47:30.412606 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2024-03-25 03:04:07.866341 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      670 2024-03-25 03:04:07.866546 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2024-03-25 03:04:07.866888 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2024-03-25 03:04:07.867470 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      236 2024-03-25 03:04:07.867794 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1984 2024-03-25 03:04:07.868153 solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       90 2024-03-25 03:04:07.868658 solutions_builder-1.18.1/solutions_builder/requirements.txt
+-rw-r--r--   0        0        0    68957 2024-03-25 03:04:07.870229 solutions_builder-1.18.1/solutions_builder/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2024-03-25 03:04:07.870988 solutions_builder-1.18.1/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2637 2024-03-25 03:04:07.871475 solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2688 2024-03-25 03:04:07.871683 solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5784 2024-03-25 03:04:07.872126 solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8047 2024-03-25 03:04:07.874328 solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3129 2024-03-25 03:04:07.874720 solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2024-03-25 03:04:07.875041 solutions_builder-1.18.1/solutions_builder/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2024-03-25 03:04:07.876082 solutions_builder-1.18.1/solutions_builder/template_root/.pylintrc
+-rw-r--r--   0        0        0     4878 2024-03-25 03:04:07.876530 solutions_builder-1.18.1/solutions_builder/template_root/README.md
+-rw-r--r--   0        0        0      398 2024-03-25 03:04:07.876998 solutions_builder-1.18.1/solutions_builder/template_root/components/README.md
+-rw-r--r--   0        0        0      893 2024-03-25 03:04:07.877867 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
+-rw-r--r--   0        0        0     1101 2024-03-25 03:04:07.878112 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
+-rw-r--r--   0        0        0      111 2024-03-25 03:04:07.878424 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
+-rw-r--r--   0        0        0      240 2024-03-25 03:04:07.878829 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
+-rw-r--r--   0        0        0      571 2024-03-25 03:04:07.879408 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.880848 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
+-rw-r--r--   0        0        0      831 2024-03-25 03:04:07.881462 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
+-rw-r--r--   0        0        0      695 2024-03-25 03:04:07.881658 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2024-03-25 03:04:07.882687 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2024-03-25 03:04:07.882932 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1376 2024-03-25 03:04:07.884644 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.885395 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      754 2024-03-25 03:04:07.887849 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1006 2024-03-25 03:04:07.888076 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2243 2024-03-25 03:04:07.888314 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.889468 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2024-03-25 03:04:07.891212 solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2500 2024-03-25 03:04:07.891459 solutions_builder-1.18.1/solutions_builder/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2024-03-25 03:04:07.891699 solutions_builder-1.18.1/solutions_builder/template_root/firebase.json
+-rw-r--r--   0        0        0      484 2024-04-29 01:47:30.412898 solutions_builder-1.18.1/solutions_builder/template_root/sb.yaml
+-rw-r--r--   0        0        0       98 2024-03-25 03:04:07.892621 solutions_builder-1.18.1/solutions_builder/template_root/setup.cfg
+-rw-r--r--   0        0        0      215 2024-03-25 03:04:07.893127 solutions_builder-1.18.1/solutions_builder/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      921 2024-03-25 03:04:07.894470 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2024-03-25 03:04:07.894809 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2024-03-25 03:04:07.895330 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2024-03-25 03:04:07.895611 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2024-03-25 03:04:07.896165 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2024-03-25 03:04:07.896402 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1186 2024-03-25 03:04:07.896659 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2024-03-25 03:04:07.896925 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2024-03-25 03:04:07.897379 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2024-03-25 03:04:07.897631 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     3868 2024-03-25 03:04:07.898055 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2024-03-25 03:04:07.898338 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     3453 2024-03-25 03:04:07.898588 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     3012 2024-03-25 03:04:07.899082 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2024-03-25 03:04:07.899396 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2024-03-25 03:04:07.899720 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2024-03-25 03:04:07.900599 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      774 2024-03-25 03:04:07.900949 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2024-03-25 03:04:07.901558 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2024-03-25 03:04:07.902536 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2024-03-25 03:04:07.905914 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      678 2024-03-25 03:04:07.906314 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2024-03-25 03:04:07.906938 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2024-03-25 03:04:07.907328 solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2561 2024-03-25 03:04:07.908063 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/bastion_startup.sh
+-rw-r--r--   0        0        0     3593 2024-03-25 03:04:07.909125 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/main.tf
+-rw-r--r--   0        0        0      178 2024-03-25 03:04:07.909456 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/terraform.tfvars
+-rw-r--r--   0        0        0      782 2024-03-25 03:04:07.910038 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/variables.tf
+-rw-r--r--   0        0        0     2873 2024-03-25 03:04:07.910583 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2024-03-25 03:04:07.910858 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       86 2024-03-25 03:04:07.911144 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2024-03-25 03:04:07.911400 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      869 2024-04-29 01:47:30.413075 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0     1669 2024-03-25 03:04:07.912198 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2024-03-25 03:04:07.912485 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     1032 2024-03-25 03:04:07.912743 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf
+-rw-r--r--   0        0        0     4602 2024-03-25 03:04:07.913103 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      991 2024-03-25 03:04:07.913405 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      921 2024-03-25 03:04:07.913735 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      724 2024-03-25 03:04:07.914076 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2839 2024-03-25 03:04:07.914408 solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.914895 solutions_builder-1.18.1/solutions_builder/template_root/tests/__init__.py
+-rw-r--r--   0        0        0     1386 2024-03-25 03:04:07.915482 solutions_builder-1.18.1/solutions_builder/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      952 2024-03-25 03:04:07.915993 solutions_builder-1.18.1/solutions_builder/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0      990 2024-03-25 03:04:07.916378 solutions_builder-1.18.1/solutions_builder/template_root/utils/init_env_vars.sh
+-rwxr-xr-x   0        0        0     1845 2024-03-25 03:04:07.917312 solutions_builder-1.18.1/solutions_builder/template_root/utils/setup_ksa.sh
+-rw-r--r--   0        0        0       81 2024-03-25 03:04:07.917579 solutions_builder-1.18.1/solutions_builder/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2024-03-25 03:04:07.917901 solutions_builder-1.18.1/solutions_builder/tests/__init__.py
+-rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 solutions_builder-1.18.1/PKG-INFO
```

### Comparing `solutions_builder-1.18.0/LICENSE` & `solutions_builder-1.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/README.md` & `solutions_builder-1.18.1/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/pyproject.toml` & `solutions_builder-1.18.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-builder"
-version = "1.18.0"
+version = "1.18.1"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-builder"
 repository = "https://github.com/GoogleCloudPlatform/solutions-builder"
 packages = [
```

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/cli.py` & `solutions_builder-1.18.1/solutions_builder/cli/cli.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/cli_constants.py` & `solutions_builder-1.18.1/solutions_builder/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/cli_utils.py` & `solutions_builder-1.18.1/solutions_builder/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/component.py` & `solutions_builder-1.18.1/solutions_builder/cli/component.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/infra.py` & `solutions_builder-1.18.1/solutions_builder/cli/infra.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/set.py` & `solutions_builder-1.18.1/solutions_builder/cli/set.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/template.py` & `solutions_builder-1.18.1/solutions_builder/cli/template.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/vars.py` & `solutions_builder-1.18.1/solutions_builder/cli/vars.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/cli/vars_test.py` & `solutions_builder-1.18.1/solutions_builder/cli/vars_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/copier_extensions/context.py` & `solutions_builder-1.18.1/solutions_builder/copier_extensions/context.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/copier_extensions/sb_helpers.py` & `solutions_builder-1.18.1/solutions_builder/copier_extensions/sb_helpers.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/README.md` & `solutions_builder-1.18.1/solutions_builder/module_template/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/module_template/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/template_copier.yaml` & `solutions_builder-1.18.1/solutions_builder/module_template/template_copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml` & `solutions_builder-1.18.1/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf` & `solutions_builder-1.18.1/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/Dockerfile` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/README.md` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/main.py` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/routes/sample.py` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/src/routes/sample.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/1.0/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/blank_service/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/blank_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/README.md` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/README.md` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/README.md` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/backend.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/iam.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/main.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/providers.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/variables.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke/terraform/stages/{{terraform_stage_name}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/docs/components/{{component_name}}.md` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/docs/components/{{component_name}}.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/backend.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/main.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/providers.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/variables.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_autopilot/terraform/stages/{{terraform_stage_name}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/backend.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/iam.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/main.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/providers.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/terraform.tfvars` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/variables.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_gke_ingress/terraform/stages/{{terraform_stage_name}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_builder-1.18.1/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/setup_local.png` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/.pylintrc` & `solutions_builder-1.18.1/solutions_builder/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/README.md` & `solutions_builder-1.18.1/solutions_builder/template_root/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py` & `solutions_builder-1.18.1/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/copier.yaml` & `solutions_builder-1.18.1/solutions_builder/template_root/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/firebase/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/firebase/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/firebase/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/outputs.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/gke/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/gke/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/project_services/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/project_services/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/project_services/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/service_account/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/service_account/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/service_account/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/vpc_network/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/bastion_startup.sh` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/bastion_startup.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/0-jumphost/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/0-jumphost/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/identity_platform.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/main.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_builder-1.18.1/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/tests/e2e/e2e_utils.py` & `solutions_builder-1.18.1/solutions_builder/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/utils/disable_org_policies.sh` & `solutions_builder-1.18.1/solutions_builder/template_root/utils/disable_org_policies.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/utils/init_env_vars.sh` & `solutions_builder-1.18.1/solutions_builder/template_root/utils/init_env_vars.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/solutions_builder/template_root/utils/setup_ksa.sh` & `solutions_builder-1.18.1/solutions_builder/template_root/utils/setup_ksa.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.18.0/PKG-INFO` & `solutions_builder-1.18.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solutions-builder
-Version: 1.18.0
+Version: 1.18.1
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-builder
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

