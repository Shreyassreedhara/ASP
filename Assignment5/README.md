# Assignment 5

This program tests a user app that uses the character device driver that I have written. Following are the instructions on how you can run this program on your system.

1. Clone the repository into your local machine
2. Traverse to the Assignment5 folder
3. Open the command line from that directory and become super user by using the following command:
```
sudo su
```
* It is neccessary to become the super user so that we can load the driver that we have written

4. Compile the driver module using the command:
```
make
```
5. Compile the userapp using the following command:
```
make app
```
6. Load the module:
```
insmod char_driver.ko <num_devices>
```
* Here the 'num_devices' is a number of your choice. The number you give here is the number of devices that your driver will support
7. Test the driver
   - Run userapp:
   ```
   ./userapp <device_number>
   ```
   * Here the device number specifies the id number of the device to be tested
   - Choose the appropriate function when prompted and also choose the offset if prompted 
8. Once the testing is done, use this command to unload the module:
```
rmmod char_driver.ko
```
_Note:_
* Userapp has to be executed with root previleges as the device files in /dev/ are created in the driver with root previleges