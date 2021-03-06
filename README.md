# A color picker seekbar for android apps.

## Download
 - Use Gradle
```
compile 'com.karthikeyanjkk.colorseekbar:colorseekbar:1.0.2'
```
- or Maven

```
<dependency>
  <groupId>com.karthikeyanjkk.colorseekbar</groupId>
  <artifactId>colorseekbar</artifactId>
  <version>1.0.2</version>
  <type>pom</type>
</dependency>
```

## Usage

 - XML
 ```
 <com.karthikeyanjkk.colorseekbar.ColorSeekBar
        android:id="@+id/color_seek_bar"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_margin="16dp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent" />
```

- Attributes

<table>
 <th>Attribute Name</th>
 <th>Description</th>
 <tr>
    <td>app:colorSeeds="@array/colors"</td>
    <td>Set the colors of seekbar</td>
 </tr>
  <tr>
    <td>app:cornerRadius="4dp"</td>
    <td>Sets the corner radius of bar.</td>
 </tr> 
 <tr>
    <td>app:barHeight="8dp</td>
    <td>Sets the height of color bar.</td>
 </tr>
  <tr>
    <td>app:thumbBorder="4dp"</td>
    <td>Sets the width of thumb border.</td>
 </tr>
  <tr>
    <td>app:thumbBorderColor="@android:color/black"</td>
    <td>sets the color of thumb border.</td>
 </tr>
 </table>
 
 - Listener
 
 ```
 color_seek_bar.setOnColorChangeListener(object: ColorSeekBar.OnColorChangeListener{
            override fun onColorChangeListener(color: Int) {
                //gives the selected color
                view.setBackgroundColor(color)
            }
        })
```
## Connect

- [Twitter](https://twitter.com/karthikeyanjkk)
- [Medium](https://medium.com/@karthikeyanjkk)

## LICENCE
```
Copyright 2021 karthikeyanjkk

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
