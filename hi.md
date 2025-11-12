# GCP Infrastructure Setup Commands

All resources are created in the **us-east4** region and **us-east4-c** zone.

---

## 1. Create a Cloud Storage Bucket
```bash
gsutil mb -p [PROJECT_ID] -l us-east4 -b on gs://[UNIQUE_BUCKET_NAME]/
