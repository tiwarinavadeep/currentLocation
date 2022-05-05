# currentLocation


//add dependency to your build.gradel file

        implementation 'com.github.tiwarinavadeep:CurrentLocation:1.0.1'

//In Your Activity Class

        LocationHelper
        .startWith(this)
        .lastKnownLocation{lastLocation->

                //null check for last location

                lastLocation?.let {
                        //here you found your last location
                        Log.d("lastLocation", it.fullAddress?:"")
                 }
        }

