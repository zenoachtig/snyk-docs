# Add images to Snyk from GCR

Snyk tests and monitors Google Container Registry (GCR) container images by evaluating root folders and custom file locations.

## **Prerequisites for adding images to Snyk from GCR**&#x20;

* You must have an account with Snyk and be onboarded to your Organization by an administrator.
* The integration must be configured between Snyk and your GCR repository.

## Steps to add images to Snyk from GCR&#x20;

Log in to your account and navigate to the relevant Group and Organization you want to manage.

Go to **Projects** and click **Add projects**. The list of integrations already configured in your account opens.&#x20;

Decide which images you want to test. The view displays all of the available images for the registry to which you connected, grouped by each of your repositories, similar to the following:

Continue with the following steps:

1. Select single or multiple images by using any or all of the following methods:
   * Type the name of a single image for import in the **Image Name** field.
   * Select any of the repositories for which you want to import all of the associated images.
   * Expand and collapse repositories to select multiple images across multiple repositories.
2.  Click **Add selected repositories**.

    A status bar appears at the top of the page as the images are imported; you can continue working while the images are being imported.
3. When the import ends, a notification of success or failure appears at the top of the page. Click **Refresh** to view the **Projects** page with the newly imported images. Images are grouped by repository and are each linked individually to a detailed Projects page.
4. You can now connect your Git repo to this Project in order to use your Dockerfile for enriched fix advice. For more information, see [Adding your Dockerfile and testing your base image](../../scan-your-dockerfile/detect-vulnerable-base-images-from-your-dockerfile.md).

GCR files are indicated with a unique icon. You can now filter to view only those Projects.

<figure><img src="../../../../.gitbook/assets/Screenshot 2023-03-31 at 18.06.20.png" alt=""><figcaption><p>Examples of GCR Projects</p></figcaption></figure>

GCR integration works similarly to other Snyk integrations. To continue to monitor, fix, and manage your Projects, see the relevant pages in the Snyk docs.

{% hint style="info" %}
For application vulnerabilities within container images, any changes to the application will not be reflected with a manual or recurring retest. You must re-import the image. For more information, see [Detecting application vulnerabilities in container images](../../use-snyk-container/detect-application-vulnerabilities-in-container-images.md).
{% endhint %}
