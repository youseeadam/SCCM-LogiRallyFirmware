# SCCM-LogiRallyFirmware
<ol>
  <li>Download the file Logitech.Rally.Firmware.Updater.zip</li>
  <li>Copy the "Logitech Rally Firmware Updater_files" to your distribution share</li>
  <li>Import the "Logitech Rally Firmware Updater.zip" into your SCCM applications</li>
  <li>When you import the configuration an error will occure, choose to ignore the errors</li>
  <li>Go the properties of the Application</li>
  <li>Edit the deployment type of "Logitech Rally Firmware Updater"</li>
  <li>Change the Content location to match your configuration (where you extracted the Logitech Rally Firmware Updater_files above)</li>
  <li>In the command to install, you can change the rightsight to the following<br>
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
  <li>You will want to download the latest version of the firmware from Logitech Support site</li>
  </ul>
  
