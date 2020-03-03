# SCCM-LogiRallyFirmware
<ol>
  <li>Download the file Logitech.Rally.Firmware.Updater.zip</li>
  <li>Extract the file to your distribution point on your DP. In this example it is \\sccm2\applications. This means there will be two sub items created</li>
  <ul>
    <li>Logitech Rally Firmware Updater_files</li>
    <li>Logitech Rally Firmware Updater.zip</li>
  </ul>
  <li>Import the "Logitech Rally Firmware Updater.zip" into your SCCM applications</li>
  <li>During the import at the verification staage make sure that Logitech Rally System Detection, Logitech Rally System Firmware 1.4.28 and The Logitech Software Category are all set to Create New</li>
  <li>At this point you can delete the Logitech Rally Firmware Updater.zip</li>
  <li>Go the properties of the Application</li>
  <li>Go to the content tab, notice the location of the content will have the file location with a GUID, similar to this: \\sccm2\applications\Logitech Rally Firmware Updater_files\Content_484bd7b2-3706-489d-9bef-5f33d6339f44. You can leave this as is, or move the file to a different location or name. If you do, you will need to update the Content Location.</li>
  <li>In the programs tab, you can change the rightsight to the following<br>
    <blockquote>
      Dynamic (Defualt)<br>
      OCS (On Call Start, frame only at the begging of the meeting<br>
      Off
      </blockquote>
  <li>Deploy and Distribute the application</li>
  </ol>
  <B>Notes:</B>
<ul>
  <li>This application will import an condition to detect if the Rally is connected, this will ensure it only is deployed to devices with a Rally attached. If you do not want this condition remove the requirment from the application deployment type.</li>
  <li>You will want to download the latest version of the firmware from Logitech Support site. If you do download a newer version, make sure to rename the file to FWUpdateRally.exe and change the name of the application.</li>
  </ul>
  
