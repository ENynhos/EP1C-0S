# First step
 You need to download the GRUB directory from this page 

# Second step
  Just copy the directory into you /boot/grub/themes/
  if you dont have the /themes you can just copy to the /grub/

    sudo cp /home/yourName/Downloads/EPIC-OS /boot/grub/themes/

  # Third step
  Now you must edit the /etc/default/grub changing the GRUB_THEME path
  to where you put the EPIC-OS directory and specifiying the theme.txt file in the path
     
     sudo nano(or any text editor you use) /etc/default/grub
  
  ## EX:
    GRUB_THEME="/boot/grub/themes/EPIC-OS/theme.txt"
  ### OBS
  as default the GRUB_THEME is marked as comment you neet to delete the # before the GRUB_THEME

  # Now you just need to update you grub and reboot
  you can simply do this by using 

      sudo update-grub

  or if this doesnt work you can run

      sudo grub-mkconfig -o /boot/grub/grub.cfg

  now just reboot and enjoy your **EPIC** GRUB!
