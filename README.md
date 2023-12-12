<!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages).
-->

TODO: This package will help the Developer to implement Searchable Dropdown with alot more features like clear seleciton on 
button click fetch values from sqlite.

## Features

TODO: This package will help the Developer to implement Searchable Dropdown with alot more features like clear seleciton on
button click fetch values from sqlite.

## Getting started

TODO: This package will help the Developer to implement Searchable Dropdown with alot more features like clear seleciton on
button click fetch values from sqlite.

## Usage

TODO: I have add the very very useful example. Add longer examples
to `
SearchableDropDownClearSelection(
showClearButton:true,

                    items: _citiesList,
                    label: 'Select parcel Id',
                    decoration:
                        BoxDecoration(border: Border.all(color: Colors.blue)),
                    prefixIcon: Padding(
                      padding: const EdgeInsets.all(0.0),
                      child: Icon(Icons.search),
                    ),
                    dropDownMenuItems: _citiesList?.map((item) {
                          return item.toString();
                        })?.toList() ??
                        [],
                    onChanged: (value) {
                      if (value != null) {
                        spn_parcel_no_firstValue = value;

                        if (spn_parcel_no_firstValue != "Select Parcel Id") {
                          print("city1= $spn_parcel_no_firstValue");
                          setState(() {
                          isErrorConditionMetParcelId = false;
                        });
                        }else{
                          print("else2= $spn_parcel_no_firstValue");

                          spn_parcel_no_firstValue = 'Select Parcel Id';

                        }
                      } else {
                        print("else1= $spn_parcel_no_firstValue");

                        spn_parcel_no_firstValue = 'Select Parcel Id';
                        }
                    },
                    onClearPressed: () {
                      // Handle clear button press
                      print('Clear button pressed');
                      // Reset the selected value to an initial state (e.g., null)
                      // setState(() {
                      //   selectedValue = null;
                      // });
                    },

                  )` folder.

```dart
const like = 'sample';
```

## Additional information

TODO: You can easily find the package in pub.dev.
