# Node Sample App

This Repo will explain how to run the Node Sample App.

### Pre-requisites

- Git
- Virtual Box
- Vagrant

### Running the app


1) `vagrant up` This launches both VMs, and provisions them.

2) `vagrant ssh app` This grants you access to the VM.

3) `cd /home/ubuntu/app` This is where the app is stored within the VM

4) `npm install` This is installs npm and allows for npm commands such as start and test to work.

5) `npm start` This will active the app and allow you to use your web browser to access the App

6) In your web browser, go to `development.local` to access the app

7)You should now see the app! Here you have a few options:
 - `/posts` allows you to see the posts from the app
 - `/fibonacci/<index>` where `<index>` is a number. This will produce the number associated with your value in the fibonacci sequence.

#### Tests

##### App

To run the tests inside the app run:
```
npm test
```
###### Local

To run the tests locally, outside the VM, from the root directory:
```
cd tests
rake spec:app
rake spec:db
```
