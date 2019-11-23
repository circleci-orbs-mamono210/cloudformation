# Test Decision Table

## create-stack

| Parameter | Value | Rule1 | Rule2 | Rule3 | Rule4 | Rule5 | Rule6 |
| ---- |:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| **aws-access-key-id** | *Default / String* | D | D | D | D | S | S |
| **aws-region** | *Default / String* | D | D | D | D | S | S |
| **aws-secret-access-key** | *Default / String* | D | D | D | D | S | S |
| **branch** | *No Value / String* | N | N | N | S | S | S |
| **configure-default-region** | *True / False* | T | T | T | T | T | F |
| **extra-arguments** | *No Value / String* | N | S | S | S | S | S |
| **git-url** | *No Value / String* | N | N | S | S | S | S |
| **profile-name** | *Default / String* | D | D | D | D | S | S |
| **stack-name** | *String(Required)* | S | S | S | S | S | S |
| **template-file-path** | *String(Required)* | S | S | S | S | S | S |


## delete-stack

| Parameter | Value | Rule1 | Rule2 | Rule3 | Rule4 | Rule5 | Rule6 |
| ---- |:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| **aws-access-key-id** | *Default / String* | D | D | D | D | S | S |
| **aws-region** | *Default / String* | D | D | D | D | S | S |
| **aws-secret-access-key** | *Default / String* | D | D | D | D | S | S |
| **configure-default-region** | *True / False* | T | T | T | T | T | F |
| **extra-arguments** | *No Value / String* | N | S | S | S | S | S |
| **profile-name** | *Default / String* | D | D | D | D | S | S |
| **stack-name** | *String(Required)* | S | S | S | S | S | S |
| **template-file-path** | *String(Required)* | S | S | S | S | S | S |


## deploy

| Parameter | Value | Rule1 | Rule2 | Rule3 | Rule4 | Rule5 | Rule6 |
| ---- |:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| **aws-access-key-id** | *Default / String* | D | D | D | D | S | S |
| **aws-region** | *Default / String* | D | D | D | D | S | S |
| **aws-secret-access-key** | *Default / String* | D | D | D | D | S | S |
| **branch** | *No Value / String* | N | N | N | S | S | S |
| **capabilities** | *No Value / String* | N | N | N | S | S | S |
| **configure-default-region** | *True / False* | T | T | T | T | T | F |
| **extra-arguments** | *No Value / String* | N | S | S | S | S | S |
| **git-url** | *No Value / String* | N | N | S | S | S | S |
| **parameter-overrides** | *No Value / String* | N | N | S | S | S | S |
| **profile-name** | *Default / String* | D | D | D | D | S | S |
| **stack-name** | *String(Required)* | S | S | S | S | S | S |
| **template-file-path** | *String(Required)* | S | S | S | S | S | S |


## describe-stack

| Parameter | Value | Rule1 | Rule2 | Rule3 | Rule4 | Rule5 | Rule6 |
| ---- |:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| **aws-access-key-id** | *Default / String* | D | D | D | D | S | S |
| **aws-region** | *Default / String* | D | D | D | D | S | S |
| **aws-secret-access-key** | *Default / String* | D | D | D | D | S | S |
| **configure-default-region** | *True / False* | T | T | T | T | T | F |
| **extra-arguments** | *No Value / String* | N | S | S | S | S | S |
| **profile-name** | *Default / String* | D | D | D | D | S | S |
| **stack-name** | *String(Required)* | S | S | S | S | S | S |
