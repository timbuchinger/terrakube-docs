# GitLab

For using repositories from Gitlab.com with Terrakube workspaces and modules you will need to follow these steps:

{% hint style="info" %}
**Manage VCS Providers** permission is required to perform this action, please check [team-management.md](../organizations/team-management.md "mention") for more info.
{% endhint %}



Navigate to the desired organization **** and click the **Settings** button, then on the left menu select **VCS Providers**&#x20;

<figure><img src="../../.gitbook/assets/image (14) (2).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If you prefer, you can add a new VCS Provider directly from the Create workspace or Create Module screen.&#x20;
{% endhint %}

Click the **Gitlab button**

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

In the next screen click the link to [register a new OAuth Application](https://gitlab.com/-/profile/applications) in Gitlab

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

On Gitlab, complete the required fields and click **Save application** button

| Field        | Description                                                            |
| ------------ | ---------------------------------------------------------------------- |
| Name         | Your application name, for example you can use your organization name. |
| Redirect URI | Use https://localhost we will update this value later                  |
| Scopes       | Only **api** should be checked                                         |

{% hint style="info" %}
You can complete the fields using the information suggested by terrakube in the VCS provider screen
{% endhint %}

<figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

In the next screen, copy the **Application ID** and **Secret**

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

Go back to Terrakube to enter the information you copied from the previous step. Then, click the **Connect and Continue** button.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

In the next screen copy the **Callback URL,** we will need this value to update our gitlab application

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Go back to Gitlab and update the Redirect URI, click the **Save application** button

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Once you updated the Callback Url in Gitlab, return to Terrakube and click the **Connect to Gitlab** button

<figure><img src="../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

You will see a new window, click the **Authorize** button to complete the connection

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Finally if the connection was stablished successfully, you wil see a **Connected** message, you can close the window and return to Terrakube.

<figure><img src="../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

If you refresh the VCS providers page in your organization, you should see the connection status with the date and the user that created the connection

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

And now, you will be able to use the connection in your workspaces and modules:

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>