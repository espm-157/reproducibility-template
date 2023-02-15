# A Reproducibility Tutorial

## Getting Started on GitHub Codespaces

*Please Note: Codespaces seems to fail to start in Safari. Please try Chrome or Firefox*

### My Students

In my tutorials, I will provide a 'magic link' that is the equivalent of the "Use Template" option outlined below for Anyone.

The only difference is that the 'magic link' will create a repository in our course GitHub Organization rather than a location that you choose (such as your own GitHub account). Being associated with the course organization lets the course lets us benefit from Educational Account features and resources, and ensures that I as your instructor have access to private repositories in the Org account. I cannot troubleshoot issues or permissions in repositories where I am not granted access. Click on the magic link I have provided to get started, then proceed to the directions for "Anyone" starting at Step 2.

### Anyone

Anyone can deploy this repository in codespaces by taking advantage of the current [free tier available for all users](https://docs.github.com/en/billing/managing-billing-for-github-codespaces/about-billing-for-github-codespaces), or by using their own codespaces subscription.

#### Step 1:

Click on the green button saying "Use this template". Choose a location (i.e. your own GitHub account) and name for your new repository. This should bring you to a new repository based on this template! It will look nearly the same, but be under a different URL where you can store (push) your work. Instead of a "Use this template" button, you will now see the green button says "\<\> Code" (see step 2).

![](https://user-images.githubusercontent.com/222586/218885361-269658a0-308e-4f4f-972e-d918f9cd90de.png)

#### Step 2:

You should now be in your own repository where the Green button says "\<\> Code" (see screenshot below, lower right)

![](https://user-images.githubusercontent.com/222586/218886058-3902196e-f5a0-4345-b2e4-40b4798dd463.png)

Click Code, select the codespaces tab, and click "**Create codespace on main**" (screenshot below. Note only my students will see the "Codespace paid for by espm-288")

![](https://user-images.githubusercontent.com/222586/218886220-e5d25c1d-2ec4-49ef-ad04-bd5a0191672e.png)

Note: if you already have an active codespace on this repository, it will appear here. If you have too many open codespaces on this or other repository, you may not be able to make a new one until you remove some old ones, see <https://github.com/codespaces> to manage your open codespaces.

#### Step 3 (Optional):

The Codespace takes several minutes to start on first use, and will launch into a virtual machine running a customized Visual Studio Code interface.

Users that prefer the RStudio interface can access it by clicking on the Ports tab (this may take another minute to appear after the instance opens), and clicking on the "globe" icon to open the link. This should open a new tab showing an RStudio login page.

![](https://user-images.githubusercontent.com/222586/218887216-f121d03b-edc0-423c-a455-ab361bee1adc.png)

The default login user/password here is rstudio/rstudio.

![](https://user-images.githubusercontent.com/222586/218887796-7f7a0379-0b65-48e0-b318-de102b55ed71.png)

Once RStudio opens, consider using `File -> New Project -> Existing Directory` and selecting the directory matching your repository name. This should get you in the correct workspace with an active "git" tab for version control.

![](https://user-images.githubusercontent.com/222586/218887914-6a34dca5-7c02-43a4-92c5-90ef72134cca.png)
