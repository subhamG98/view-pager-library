Android View Pager Library
======

#### This Library can be used to create view pager in android very easily.
#### View Pager is a Layout element that helps users to slide images one after the other.
#### In this Library only one function is used and can be customized to user needs.
![alt text](https://github.com/subhamG98/view-pager-library/blob/master/ScreenRecorder_Exported_20160905182113.gif "Now you have to just select the images and transition speed ,rest all will be done.")


# Download:

Maven:
<dependency>
  <groupId>com.example.mypc.mylibrary</groupId>
  <artifactId>mylibrary</artifactId>
  <version>1.0</version>
  <type>pom</type>
</dependency>

# Gradle:

## compile 'com.example.mypc.mylibrary:mylibrary:1.0'


---
---

Here you can see the sample java file where you can use this function.


public class MainActivity extends Activity {
    int[] imageId = {
            R.drawable.b1,
            R.drawable.b2,
            R.drawable.b3,
            R.drawable.b2,
            R.drawable.b1,
            R.drawable.b3



    };

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        View v = new MyView(this);
        setContentView(v);


        MyView.addViewPager(5, MainActivity.this,imageId,100,3000);
        
        //Here first param is no of images
        // second is activtity
        // third is images array
        // fourth is speed of transition
        // fifth is duration for one image to stay.
        

    }




## License:


Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
