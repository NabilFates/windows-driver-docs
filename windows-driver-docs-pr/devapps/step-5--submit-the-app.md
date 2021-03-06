---
title: Step 5 Submit the Windows Store device app
description: This topic describes how to submit your Windows Store device app to the Windows Store dashboard.
ms.assetid: B25F9953-6EFD-4A08-AFD6-B334C46E910F
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Step 5: Submit the Windows Store device app


![device app workflow, step 5](images/5-device-app-workflow.png)

This topic describes how to submit your Windows Store device app to the Windows Store dashboard. Before submitting your app, review the submission sequence section in [Building Windows Store device apps](the-workflow.md). This topic is part of a step-by-step series. See [Build a Windows Store device app step-by-step](build-a-windows-store-device-app-step-by-step.md) for the introduction.

**Note**  If your app is specified as a privileged app and it is not configured for automatic installation, you can submit your device metdata to the Windows Dev Center hardware dashboard before you submit your privileged app to the Windows Store. In this case, this step 5 can take place after [step 6](step-6--submit-device-metadata.md).

 

A Windows Store device app is a special kind of Windows Store app that device manufacturers create to serve as a companion to their internal or peripheral device. By using device metadata, device apps can run privileged operations, such as device update. For more info about Windows Store device apps, see [Meet Windows Store device apps](meet-windows-store-device-apps.md).

## <span id="Before_you_begin"></span><span id="before_you_begin"></span><span id="BEFORE_YOU_BEGIN"></span>Before you begin


This topic assumes that you've finished developing your app and the device metadata is ready to go.

## <span id="Start_app_submission"></span><span id="start_app_submission"></span><span id="START_APP_SUBMISSION"></span>Start app submission


Go to the [Windows Store dashboard](http://go.microsoft.com/fwlink/p/?LinkId=273050) and click **Submit a new app**.

## <span id="Add_instructions_for_testers"></span><span id="add_instructions_for_testers"></span><span id="ADD_INSTRUCTIONS_FOR_TESTERS"></span>Add instructions for testers


In the **Instructions for testers**, make sure that you enter the text "This is a Windows Store device app." This indicates to the app submission testers that your app is a Windows Store device app.

## <span id="Review_submission_details"></span><span id="review_submission_details"></span><span id="REVIEW_SUBMISSION_DETAILS"></span>Review submission details


Check the following before you submit your app:

-   The description of the app should clearly state the hardware that the app requires.

-   You must include the StoreManifest.xml file in the app package for the Windows Store to recognize the app as a Windows Store device app.

-   When the app is launched, if the app requires that the device be connected before the app will work, it must clearly state something like "Please connect your &lt;*brand-specific device name*&gt;".

-   The **package name** should be the same as the one you specified when you created the app in [step 1](step-1--create-a-windows-store-device-app.md). Note that the package name expires if the app is not submitted within one year.

-   The app must be fully compliant with all the [Windows Store Certification Requirements](http://go.microsoft.com/fwlink/p/?LinkId=273052).

-   The app must be suitable for all ages.

-   The app must be marked as free.

## <span id="Confirm_selling_details"></span><span id="confirm_selling_details"></span><span id="CONFIRM_SELLING_DETAILS"></span>Confirm selling details


During app submission, check the **Selling Details** item in the Store submission checklist, and ensure that you see this:

**Your app must be free because it is a Windows Store device app.**

**Your app will sell for Free and is schedued for release after it passes certification.**

The app submission UI is designed to look for StoreManifest.xml as the only means of checking whether the app is a Windows Store device app associated with a device. And once it makes that determination, it will explicitly override whatever you set in the selling details to make sure the app is set to be free with no trial (and disable the controls if you try to change those values in the **Selling Details** page). This is then reflected on the checklist page.

If you don't see **Your app must be free because it is a Windows Store device app** in the **Selling Details** page, check that you have correctly included StoreManifest.xml in the root folder of your app project, and not in the solution’s root folder.

## <span id="Submission_results"></span><span id="submission_results"></span><span id="SUBMISSION_RESULTS"></span>Submission results


Once the Windows Store receives your app, it will perform a suite of automated tests that are common to all Windows Store apps. It will also perform a series of tests that are specific to the app.

If your app passes the tests applied by the Windows Store, it will be added to the App Catalog in about 1-4 days. Once it's in the Catalog, it's available from the Windows Store as well. If submission fails, you’ll be notified as to the cause.

## <span id="Validation"></span><span id="validation"></span><span id="VALIDATION"></span>Validation


The Windows Store dashboard validates the Windows Store device app package after it’s submitted to the Windows Store. Device metadata is submitted to and validated by the Windows Dev Center hardware dashboard. You should submit the metadata after the app is live on the Windows Store, because the validation process checks that the app specified in the metadata is in the Store. The hardware dashboard validates drivers separately, as part of a Logo submission.

## <span id="Next_step"></span><span id="next_step"></span><span id="NEXT_STEP"></span>Next step


[Step 6: Submit device metadata](step-6--submit-device-metadata.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[devapps\devapps]:%20Step%205:%20Submit%20the%20Windows%20Store%20device%20app%20%20%20RELEASE:%20%281/20/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




