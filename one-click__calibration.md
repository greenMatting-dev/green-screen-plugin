
- There are two types of green screen calibration: full green screen calibration and one-click green screen calibration. 
- Full green screen calibration involves only a green screen with no other objects in the frame. One-click green screen calibration involves a one-click intelligent calibration when there are people and objects in the frame.

- Lan Song Cutout uses one-click intelligent calibration. The explanation is as follows:
Full green screen calibration: When a person is not in the frame, the light shines directly onto the green screen. In this case, the calibration image is a bright green screen image. However, when a person walks in, the light shines on them, and their shadow is reflected on the green screen behind them, significantly reducing the brightness of the green screen. Even with background lighting, the shadow of the person in the foreground will still dim the color of the green screen. This results in a significant difference between the green color of the calibration image and the green screen image during the live cutout, resulting in an unclean cutout.
When a person is in the frame, the color of the green screen behind them is the green color of the combined background and foreground light, representing the live broadcast image. During calibration, the calibrated image becomes the current image. This image is used as a reference for green keying, and image operations are then performed with subsequent images to ensure a clean keying.

Alternatively, if the user is broadcasting from a seated position, with a row of immovable chairs and products in front of them, full green screen calibration is not possible, and one-click smart calibration is the only option.

Lan Song Cutout has developed an intelligent one-click calibration method. This uses an AI algorithm to identify the current person and surrounding objects, and through various operations, generates a clean, pure green calibration image. This calibration image, combined with the image, can be used for green keying to eliminate wrinkles and noise.


Tips:
Why is green keying necessary? It is currently recognized as the best green keying method in the industry, both domestically and internationally. Whether using professional film and television post-production software Nuke or hardware keyer BMD, using a calibration image can largely avoid uncertainties caused by camera imaging, lighting layout, and other factors. If you don't use a calibration chart and instead use a point-based method, such as with Keylight or the built-in green cut filter in OBS, you'll need a much smoother image, with more uniform lighting and camera imaging, ideally. However, in practice, it's impossible to cleanly cut out every area of the image at once. (Keylight is a post-production software that uses multiple keylights to achieve a clean cut, which is different from live streaming.)
For more information, we recommend downloading the Bluesong Cutout plugin for a hands-on demo, or opening the Bluesong Technical Documentation.
