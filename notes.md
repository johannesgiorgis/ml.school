# Notes

## Setup

```sh
aws s3 cp program/penguins.csv s3://jgiorgis-mlschool/penguins/data/data.csv
```

## Assignments

```python
# within bpython
for i in range(1, 6):
    for j in range(1, 6):
        print(f"- [ ] {i}.{j}")
```

- [x] 1.1
- [x] 1.2
- [x] 1.3
- [ ] 1.4 - complete later
- [ ] 1.5 - complete later
- [x] 2.1
- [ ] 2.2
- [ ] 2.3
- [ ] 2.4
- [ ] 2.5
- [ ] 3.1
- [ ] 3.2
- [ ] 3.3
- [ ] 3.4
- [ ] 3.5
- [ ] 4.1
- [ ] 4.2
- [ ] 4.3
- [ ] 4.4
- [ ] 4.5
- [ ] 5.1
- [ ] 5.2
- [ ] 5.3
- [ ] 5.4
- [ ] 5.5

## Dev Notes

```sh
λ  aws sagemaker list-model-package-groups
{
    "ModelPackageGroupSummaryList": [
        {
            "ModelPackageGroupName": "penguins",
            "ModelPackageGroupArn": "arn:aws:sagemaker:us-west-2:891067072053:model-package-group/penguins",
            "CreationTime": "2024-03-11T20:17:24.722000-07:00",
            "ModelPackageGroupStatus": "Completed"
        }
    ]
}


λ  awss list-model-packages --model-package-group-name penguins
{
    "ModelPackageSummaryList": [
        {
            "ModelPackageGroupName": "penguins",
            "ModelPackageVersion": 1,
            "ModelPackageArn": "arn:aws:sagemaker:us-west-2:891067072053:model-package/penguins/1",
            "CreationTime": "2024-03-11T20:17:25.105000-07:00",
            "ModelPackageStatus": "Completed",
            "ModelApprovalStatus": "Approved"
        }
    ]
}

awss describe-model-package --model-package-name arn:aws:sagemaker:us-west-2:891067072053:model-package/penguins/1
```
