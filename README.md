# custom-github-actions-download
Public action for to download private custom actions

## Usage

See [action.yaml](action.yaml) for the full documentation for this action's inputs and outputs.

```yaml
steps:
- name: Download custom action
  uses: la-haus/custom-github-actions-download@master
    with:
      action-name: my-custom-action  
      s3-bucket-name: ${{ secrets.CUSTOM_ACTIONS_S3_BUCKET }}
      aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
      aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
      aws-region: ${{ secrets.AWS_REGION }}
```

## Contributors

* Esteban Cataño Escobar

## License

This project is property of La Haus