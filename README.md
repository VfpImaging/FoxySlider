# FoxySlider
A pure VFP class of a Slider control
<h1><strong>FOXYSLIDER DOCUMENTATION</strong></h1>
<p>A trackbar is a control&nbsp;that contains a slider (sometimes called a thumb) in a channel, and optional tick marks. When the user moves the slider, using either the mouse or the direction keys, the trackbar sends notification messages to indicate the change.&nbsp;</p>
<p>A&nbsp;<strong>Slider</strong>&nbsp;control has a minimum, a maximum, and an increment value. You can use the Value&nbsp;of a&nbsp;<strong>Slider</strong>&nbsp;to modify another adjustable value. For example, a&nbsp;<strong>Slider</strong>&nbsp;control can
 enable users to gradually modify volume. When users move the&nbsp;<strong>Thumb</strong>&nbsp;in one direction, the volume increases; when users move it the other direction, the volume decreases.</p>
<p><strong>FOXYSLIDER</strong> is a very lightweight control. Just toss one instance of the class in your form and set some properties!</p>
<p>The following illustration shows some examples of the slider control.</p>
<h2>Default controls look</h2>
<p><img src="FoxySlider_xSlider_Default1.png" alt="" width="534" height="250"></p>
<h2>Customize your slider!</h2>
<p><img src="FoxySlider_xSlider_Custom.png" alt="" width="309" height="542"></p>
<p>&nbsp;</p>
<p>A&nbsp;<strong>Slider</strong>&nbsp;control lets users select a value from a range of values. The following illustration shows an example of a&nbsp;<strong>Slider</strong>&nbsp;control.</p>
<p><strong>Example of a Slider Control</strong></p>
<p><img src="FoxySlider_Slider_Explain.png" alt="" width="250" height="103"></p>
<p>You can customize a&nbsp;<strong>Slider</strong>&nbsp;control by setting its properties. The following list describes some of the attributes of a&nbsp;<strong>Slider</strong>&nbsp;that you can customize:</p>
<ul>
<li>
<p>The orientation of the&nbsp;<strong>Slider</strong>, either horizontal or vertical.</p>
</li><li>
<p>The tick mark locations along the&nbsp;<strong>Slider</strong>&nbsp;track.</p>
</li><li>
<p>The display of tooltips to show the current value of the&nbsp;<strong>Slider</strong>.</p>
</li><li>
<p>The ability of the Thumb&nbsp;to either snap to tick marks or to be positioned at any point along the&nbsp;<strong>Slider</strong>.</p>
</li><li>
<p>The direction of increasing value along the&nbsp;<strong>Slider</strong>.</p>
</li></ul>
<p>For more information about how to customize a&nbsp;<strong>Slider</strong>&nbsp;control, see the individual property&nbsp;descriptions below:</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h2>Properties / Methods&nbsp;</h2>
<table width="1107" style="height:635px">
<tbody>
<tr>
<td width="147"><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">StyleControl</strong></td>
<td colspan="15" width="960">
<p>Integer (0-5), Determines the style of the Slider to be used:</p>
<ul>
<li>0 = User Images; </li><li>1 = No Arrow; </li><li>2 = Both Arrows; </li><li>3 = Top or Left Arrow; </li><li>4 = Down or Right Arrow </li></ul>
</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">Max</strong></td>
<td colspan="6">Numeric, Returns/sets the maximum value of a control</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">Min</strong></td>
<td colspan="6">Numeric, Returns/sets the minimum value of a control</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">Value</strong></td>
<td colspan="4">Numeric, Returns or sets the value</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TrackImage</strong></td>
<td colspan="8">Character, The full path and name of the image which represents the track</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ThumbImage</strong></td>
<td colspan="8">String. The full path and name of the image which represents the thumb</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ThumbImageFocused</strong></td>
<td colspan="9">Character, the full path of the Thumb Image used when the object has the mouse over it</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ThumbImageDisabled</strong></td>
<td colspan="8">Character, the full path of the Thumb Image used when the object is disabled</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">Enabled</strong></td>
<td colspan="7">Logical, Specifies if the control can respond to user generated events.</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ControlSource</strong></td>
<td colspan="7">Character, Specifies the source of data to which the control is bound</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ShowTips</strong></td>
<td colspan="14">Logical, Determines if ToolTips are shown for the slider on the specified Form. *** The form property 'ShowTips' must be set to .T. as well!!!<br>
The tooltips will be shown only when the Mouse is Clicked on the Thumb button, like the MSCTL32 control.</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ShowTipsAlways</strong></td>
<td colspan="14">Logical,&nbsp;will make the tooltips to be shown also when the mouse is not clicked</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ShowFocus</strong></td>
<td colspan="9">Logical, Indicates if the control will display a focus rectangle when the control has the focus</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">IncrementStyle</strong></td>
<td colspan="9">Integer. Returns or sets a value indicating the style of increment. 0 = increment, 1 = smooth</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">LargeChange</strong></td>
<td colspan="9">Numeric, Returns/sets the increment value when the PageDown or PageUp key is pressed</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">SmallChange</strong></td>
<td colspan="9">Numeric, Returns/sets the increment value when the left or right arrow key is pressed</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickFrequency</strong></td>
<td colspan="8">Integer, Gets or sets the interval between the Tick Marks</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">ChangeWhenFocused</strong></td>
<td>Logical,&nbsp;</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickCount</strong></td>
<td colspan="7">Integer. Returns or sets a value indicating number of lines to display</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickColor</strong></td>
<td colspan="4">Integer, Returns or sets the tic line color</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickSize</strong></td>
<td colspan="4">Integer. The size of the tic lines in pixels</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickMargin</strong></td>
<td colspan="10">Integer. The distance in pixels from border of the control to the left or top edge of the tic marks</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickStyle</strong></td>
<td colspan="14">
<p>Integer, (1-4) Returns/sets a value indicating where ticks appear on a Slider control:</p>
<ul>
<li>1 = None; </li><li>2 = Both Ticks; </li><li>3 = Top/Left; </li><li>4 = Botton/Right </li></ul>
</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_prop.gif" alt="" width="16" height="16">TickDisabledColor</strong></td>
<td colspan="5">Integer, Returns or sets the tic line disabled color</td>
</tr>
<tr>
<td><strong><img src="FoxySlider_meth.gif" alt="" width="16" height="11">Scroll</strong></td>
<td colspan="5">Event,&nbsp;Occurs when you move the slider on a&nbsp;<strong>Slider</strong>&nbsp;control, either by clicking on the control or&nbsp;using keyboard commands.&nbsp;&nbsp;You can use this event to perform calculations to manipulate controls that
 must be coordinated with ongoing changes in the&nbsp;<strong>Slider</strong>&nbsp;control.</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<h2>Usage:</h2>
<p>1 - Toss one instance of the XSLIDER class from your VCX at the Project manager into your form.</p>
<p>2 - Right click the control, select properties, select the &quot;Favorites&quot; tab, to see the properties that you can customize.</p>
<p>3 - Set the main properties: &quot;Min&quot;, &quot;Max&quot;, &quot;StyleControl&quot; and your done!!!</p>
<p><img src="FoxySlider_Slider_Config2.png" alt="" width="782" height="649"></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;<img src="FoxySlider_xSlider_Default_DesignTime.png" alt="" width="898" height="655"></p>
<p>&nbsp;</p>
<p>&nbsp;<img src="FoxySlider_xSlider_Default.png" alt="" width="899" height="655"></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</body>
