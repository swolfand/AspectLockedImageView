# AspectLockedImageView

This is a small enhancement to the regular android ImageView, the AspectLockedImageView takes obviously, an Aspect Ratio, that it will respect when it is applied to a view of predefined bounds or when set to fill screen width.

## Install
```Groovy
    compile 'com.samwolfand.aspectlockedimageview:1.0'
```

## Usage
To add the DragScaleCircleView to your application, specify com.samwolfand.aspectlockedimageview in your layout XML. make sure to set the *imageAspectRatio* attribute

```xml
         <com.samwolfand.AspectLockedImageView
            android:id="@+id/movie_item_image"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:adjustViewBounds="true"
            android:scaleType="centerCrop"
            android:src="@color/color"
            app:imageAspectRatio="@dimen/aspect_ratio"/>
```

Then in your dimens.xml define a float

```xml
<resources>
    <item name="aspect_ratio" format="float" type="dimen">.675</item>
</resources>
```

License
-------

    Copyright 2016 Sam Wolfand

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
