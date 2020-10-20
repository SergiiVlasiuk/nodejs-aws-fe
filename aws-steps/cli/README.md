### some terminal commands:

aws iam get-user --profile admin
aws iam get-user --profile deployer
aws iam get-user --user-name administrator


aws ec2 describe-hosts
aws ec2 describe-hosts --filter "Name=state,Values=available"


aws ce get-cost-and-usage \
    --time-period Start=2020-10-01,End=2020-11-01 \
    --granularity MONTHLY \
    --metrics "BlendedCost" "UnblendedCost" "UsageQuantity" \
