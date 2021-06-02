# Gatekeeper templates/constraints samples
## Official documentation

### Note: Gatekeeper must be deployed on gatekeeper-system namespace

- Applying Pod Security Policies using Gatekeeper: https://cloud.google.com/kubernetes-engine/docs/how-to/pod-security-policies-with-gatekeeper
- Deploying Gatekeeper from Marketplace: https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-marketplace-app#console
- Gatekeeper official doc: https://open-policy-agent.github.io/gatekeeper/website/docs/howto

## How to apply templates/constraints from this repository
### 1) Restrict repositories to pull image from

- Create the constraint
```
kubectl apply -f https://raw.githubusercontent.com/caiottavares/gatekeeper/main/allowedRepos/constraint.yaml
```

- Create the template
```
kubectl apply -f https://raw.githubusercontent.com/caiottavares/gatekeeper/main/allowedRepos/template.yaml
```
