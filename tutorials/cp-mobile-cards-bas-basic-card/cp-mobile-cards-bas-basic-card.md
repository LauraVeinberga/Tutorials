---
parser: v2
auto_validation: true
time: 30
tags: [ tutorial>beginner, topic>mobile, operating-system>ios, operating-system>android, products>sap-business-technology-platform, products>sap-mobile-cards, products>sap-mobile-services, products>sap-business-application-studio ]
primary_tag: products>sap-mobile-cards
author_name: Sandeep T D S
author_profile: https://github.com/sandeep-tds
---

# Create Your First Card in SAP Business Application Studio
<!-- description --> Create a simple SAP Mobile Cards app by using a template, then make simple HTML modifications, and deploy the app and use it on your device.

## Prerequisites
 - [Completed the starter mission](mission.mobile-cards-get-started) or [Set up Mobile Services on your SAP Business Technology Platform account](cp-mobile-cards-setup)
 - [Set up SAP Business Application Studio for Mobile Development](cp-mobile-bas-setup)
 - **Install SAP Mobile Cards Application:**
    <table><tr><td align="center"><!-- border -->![Play Store QR Code](pre_qr_android.png)<br>Android</td><td align="center">!![App Store QR Code](pre_qr_ios.png)<br>iOS</td></tr></table>

## You will learn
  - How to create a card using a template in SAP Business Application Studio
  - How to design and develop SAP Mobile Cards in SAP Business Application Studio
  - How to deploy a card to SAP Mobile Services from SAP Business Application Studio

## Intro
Click [here](https://help.sap.com/doc/f53c64b93e5140918d676b927a3cd65b/Cloud/en-US/docs-en/guides/getting-started/mck/mck-development-bas.html) to learn more about SAP Mobile Cards in SAP Business Application Studio.

---

### Create Mobile Service connection


1. Open Business Application Studio and enter your dev workspace.

    <!-- border -->![BAS Dashboard](img_1_1.png)

2. In the menu bar, go to View &rarr; Find Command, click **Find Command**.

    <!-- border -->![Open Command Pallete](img_1_2.png)

    > For faster development, you can use the shortcut key.

3. Type *Mobile Cards* and select **Mobile Cards: Create Service Connection**.

    <!-- border -->![Service Connection Option](img_1_3.png)

4. Enter a name for your Mobile Services connection; e.g. `cf-ms-trial`.

    <!-- border -->![Service Connection Name](img_1_4.png)

5. Enter the Admin API of your Mobile Services Cockpit.

    <!-- border -->![Service Connection API](img_1_5.png)

    > You can find the Admin API in the Important Links section of your Mobile Services cockpit.

    > <!-- border -->![CPMS Important Links](img_1_5_note_1.png)

    > Upon successful connection, you will see a toast message at the bottom right corner of your screen.

    > <!-- border -->![Success toast message](img_1_5_note_2.png)


### Create a new card


1. Open Find Command, search for `Create Project from Template` and select **SAP Business Application Studio: Create Project from Template**.

    <!-- border -->![Command for New Card](img_2_1.png)

2. Select **SAP Mobile Cards** &rarr; Click **Start**.

    <!-- border -->![Command for New Card](img_2_2.png)

2. Select **Welcome Card Template - Single Instance** &rarr; Enter a name for the card; e.g. `Welcome BAS` &rarr; Click **Finish**.

    <!-- border -->![Enter a name for the card](img_2_3.png)

4. In your File Explorer, expand `Welcome BAS` Folder.

    <!-- border -->![Card Structure](img_2_4.png)

    > You can learn more about the file structure [here](https://help.sap.com/doc/f53c64b93e5140918d676b927a3cd65b/Cloud/en-US/docs-en/guides/getting-started/mck/mck-development-features.html).



### Modify the card


1. In your File Explorer, click **metadata.json**.

    <!-- border -->![Metadata.json View](img_3_1.png)

2. Add a description; e.g. **Created in SAP Business Application Studio**.

    <!-- border -->![Description View](img_3_2.png)

3. In your File Explorer, click **template_en.html**.

    <!-- border -->![HTML File view](img_3_3.png)

4. Open Find Command, search for *Mobile Cards* and select **Mobile Cards: Preview**.

    <!-- border -->![Command Pallete Preview](img_3_4.png)

    > A preview window for your card will open to the side.

    > <!-- border -->![Preview Window](img_3_4_note.png)

5. Collapse `<div class="card-content">` and replace the enclosing code inclusive of the div tags with the following code and save the file.

    ```HTML
    <div class="card-content">
      This is my first card in Business Application Studio.
    </div>
    ```

    <!-- border -->![Updated HTML File](img_3_5.png)


### Deploy and publish card


1. Open Find Command, search for *Mobile Cards* and select **Mobile Cards: Deploy**.

    <!-- border -->![Card Structure](img_4_1.png)

2. Select the card you have created; e.g. `Welcome BAS`.

    <!-- border -->![Card Structure](img_4_2.png)

    > Upon successful deployment, you will see a toast message at the bottom right corner of your screen.

    > <!-- border -->![Success toast message](img_4_2_note.png)


### Publish card in Mobile Service cockpit


1. Open your Mobile Services Cockpit.

    <!-- border -->![CPMS Cockpit](img_5_1.png)

2. Click **SAP Mobile Cards**.

    <!-- border -->![Mobile Cards Cockpit View](img_5_2.png)

3. Click on your card; e.g. `Welcome BAS`.

    <!-- border -->![Cards List](img_5_3.png)

4. In the Versions table, click the ![Publish Icon](ico_check.png) icon to change the state to **Productive**.

    <!-- border -->![Card in development status](img_5_4.png)

5. Choose **Yes** to confirm.

    <!-- border -->![Publish confirmation dialog](img_5_5.png)



### View card on your device


>Make sure you are choosing the right device platform tab ( **Android** or **iOS** ) **above**.

[OPTION BEGIN [Android]]

1. Perform **Pull Refresh** in the SAP Mobile Cards Android client.

    <!-- border -->![Android Pull Refresh](img_6_and_1.png)

    > If the card is not downloaded automatically, *re-subscribe* to the Supplier Contact Card in the All Subscriptions section.

    > <!-- border -->![Android Subscriptions View](img_6_and_1_note.png)

2. Tap on the card to open it, and notice the changes you made to the html file.

    <!-- border -->![Android Card Detail View](img_6_and_2.png)

[OPTION END]

[OPTION BEGIN [iOS]]

1. Perform **Pull Refresh** in the SAP Mobile Cards iOS client.

    <!-- border -->![iOS Pull Refresh](img_6_ios_1.png)

    > If the card is not downloaded automatically, *re-subscribe* to the Supplier Contact Card in *More &rarr; Subscriptions &rarr; All &rarr; Supplier Contact Card*.

    > <!-- border -->![iOS Subscriptions View](img_6_ios_1_note.png)

2. Tap on the card to open it, and notice the changes you made to the html file.

    <!-- border -->![iOS Card Detail View](img_6_ios_2.png)

[OPTION END]


---

**Congratulations!** You have created your first card through SAP Business Application Studio.

You can now build more [**SAP Mobile Cards apps**](https://developers.sap.com/tutorial-navigator.html?tag=products:content-and-collaboration/sap-mobile-cards) using SAP Business Application Studio.

---
