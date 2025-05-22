## Two widget 



## cold boot 
In my experience this usually happens if your emulator is set to `Quick boot`. I think there's a bug with this feature. For now, delete the device, create new emulator and in emulator options set the Boot option to `Cold boot`.

If you face this issue again, th


## image problem 

 child: Image.asset(
              'assets/passport.png',
              width: double.infinity,
              height: double.infinity,
              fit: BoxFit.cover, // or BoxFit.contain if you prefer
            ),
            after using infinity is frozen 