# kubectl-usage Plugin

## Description

`kubectl-usage` is a simple plugin for `kubectl` that prints CPU and memory usage of resources (e.g., pods) within a given namespace.

## Installation

1. Save the script as `kubectl-usage` (no `.sh` extension).
2. Make it executable:

   ```bash
   chmod +x kubectl-usage
   ```

3. Move it to a directory in your `$PATH`, for example:
   ```bash
   sudo mv kubectl-usage /usr/local/bin/
   ```
4. Now you can use it as a native `kubectl` plugin:
   ```bash
   kubectl usage <namespace> "<kubectl-command>" <resource-type>
   ```
## Example
   ```bash 
   kubectl usage top argocd pod
   ```