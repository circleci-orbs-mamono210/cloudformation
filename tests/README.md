# Test Decision Table

## create-stack

| Parameter | Value | Rule1 | Rule2 | Rule3 |
| ---- |:----:|:----:|:----:|:----:|
| **aws-access-key-id** | *Default / String* | D | D | D | D |
| **aws-region** | *Default / String* | D | D | D | D |
| **aws-secret-access-key** | *Default / String* | D | D | D | D |
| **branch** | *No Value / String* | N | N | N | S |
| **configure-default-region** | *True / False* | T | T | T | T |
| **extra-arguments** | *No Value / String* | N | S | S | S |
| **git-url** | *No Value / String* | N | N | S | S |
| **profile-name** | *Default / String* | D | D | D | D |
| **stack-name** | *String(Required)* | S | S | S | S |
| **template-file-path** | *String(Required)* | S | S | S | S |
