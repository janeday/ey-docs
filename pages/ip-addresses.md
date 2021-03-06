# IP Addresses

Engine Yard's AppCloud uses [[Amazon's Elastic IP Addresses|http://aws.amazon.com/ec2/]]. In order to use a static IP address, you need to request one via the Engine Yard AppCloud interface. You may request up to 5 IP addresses.

## Add an Address

  - From the Dashboard for your non-running environment, you click **Boot**.
  - Then for the External Address drop-down you select **Add IP Address** and a new IP address will be allocated for you and assigned this application in this environment.

## Detach an Address

You can detach an IP address from a running instance.

  - From the **IP Addresses** tab you'll see a list of your IP addresses.
  - Click on the **Detach** link, the confirmation box appears.
  - Click **OK** once you're sure.

## Attach an Address

Once you detach an IP address you can move it to a different environment.  You will need to shut down the environment before attaching it.  We recommend taking a manual snapshot of your data to help speed the termination of the environment.

### Snapshot Your Data

  - Click on the **Snapshot** button for your environment.
  - Wait until the snapshot completes.

### Boot The Instance

Now you'll reboot the instance and attach the IP address you detached above.
  - Click on **Boot** to be taken to the configuration for "your application" screen.
  - Configure your cluster for your needs.
  - For the External Address drop-down, choose the **IP address** you detached.

## Delete an Address

If you're sure you won't need an IP address anymore, you can remove it from your account.

  - Under **Server Tools** on the left, click on the **IP Addresses** tab.
  - Look for the IP address you want to delete.  
  - Then click on the **Delete** link to remove the IP address.
