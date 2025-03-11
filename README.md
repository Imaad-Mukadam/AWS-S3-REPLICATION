# AWS-S3-REPLICATION

## Summary

### **AWS S3 Replication Summary**  

1. **Create Two S3 Buckets** 🪣  
   - **Source Bucket**: Where files are initially uploaded.  
   - **Destination Bucket**: Where files will be replicated.  

2. **Enable Versioning on Both Buckets** 🔄  
   - Ensure versioning is enabled on both the source and destination buckets.  

3. **Set Up Replication Rule** 🔧  
   - Go to the **source bucket** → **Management** → **Create replication rule**.  
   - Select the **destination bucket**.  
   - Choose IAM role permissions or create a new one.  

4. **Test Replication** 📂  
   - Upload a file to the **source bucket** and check if it appears in the **destination bucket**.  

This setup ensures automatic data replication for backup or disaster recovery! 🚀

# Step - 1

i. Lets create a S3 Bucket

![image alt](1.PNG)

ii. Ensure this configuration for public access

![image alt](2.PNG)

iii. Create another bucket with same configuration (This is for Replication , you can choose another region for more avaibility)

![image alt](3.PNG)

iv. Upload your data

![image alt](4.PNG)

# Step - 2

i. Go in Management section

![image alt](5.PNG)

ii. Now, create an application rule to define where your primary bucket should transfer data during disaster recovery.

![image alt](6.PNG)

iii. Choose apply to all objects in a bucket to transfer all your data 

![image alt](7.PNG)

iv. Then browse to select your destination bucket

![image alt](8.PNG)

v. Select create a new role , then click on save

![image alt](9.PNG)

vi. Then you will see this popup , select the option based on your requirements

![image alt](10.PNG)

vii. Apply this configuration

![image alt](11.PNG)

# Step - 3

i. Upload some data in your primary bucket , then refresh in your destination bucket

![image alt](12.PNG)

