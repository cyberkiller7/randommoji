# Randmoji
This is a random generator for making fun, and wacky random Bitmoji avatars! The Node.js file uses the private API to render a completely unique Bitmoji from a list of possible attributes.

Randmoji can generate male and female Bitmoji avatars. No two avatars are similar. Every single one consists of multiple different combinations. See what funny combinations you can find!

<p align="center">
<img src="https://render.bitstrips.com//render/10225271/316830037_16_s4-v1.png?pd2={%22cranium%22:%22cranium_bm40%22,%22forehead%22:%22forehead_bm2%22,%22hair_back%22:%22hair_back_bm40%22,%22hair_front%22:%22hair_front_bm40%22,%22hairbottom%22:%22hairbottom_bm40%22,%22beard%22:%22beard_bm3_1%22,%22stachin%22:%22_blank%22,%22stachout%22:%22stachout_bm7_1%22,%22mouth%22:%22mouth_bm3%22,%22tongue%22:%22tongue_bm1_1%22,%22brow_L%22:%22brow_bm3%22,%22brow_R%22:%22brow_bm3%22,%22detail_T%22:%22detail_T_bm8%22,%22detail_L%22:%22detail_L_bm1%22,%22detail_R%22:%22detail_L_bm1%22,%22detail_E_L%22:%22detail_E_bm7%22,%22detail_E_R%22:%22detail_E_bm7%22,%22nose%22:%22nose_bm1%22,%22hat%22:%22hat_bmrasta%22,%22glasses%22:%22glasses_bm15d%22}&colours={%22ff9866%22:2571909,%22ffcc99%22:8650969,%224f453e%22:10943419,%22926715%22:6503827,%2236a7e9%22:11387424,%226f4b4b%22:4356359}&body={%22body_type%22:0}&sex=1&outfit=889235&proportion=4&cropped=%22body%22&scale=1&style=4"/> <img src="https://render.bitstrips.com//render/9946964/316830037_16_s4-v1.png?pd2={%22cranium%22:%22cranium_bm41%22,%22forehead%22:%22forehead_bm1%22,%22hair_back%22:%22hair_back_bm41%22,%22hair_front%22:%22hair_front_bm41%22,%22hairbottom%22:%22hairbottom_bm41%22,%22beard%22:%22beard_bm4_1%22,%22stachin%22:%22_blank%22,%22stachout%22:%22stachout_bm7b_1%22,%22mouth%22:%22mouth_bm5%22,%22tongue%22:%22tongue_bm1_1%22,%22brow_L%22:%22brow_bm7%22,%22brow_R%22:%22brow_bm7%22,%22detail_T%22:%22detail_T_bm5%22,%22detail_L%22:%22detail_L_bm7%22,%22detail_R%22:%22detail_L_bm7%22,%22detail_E_L%22:%22detail_E_bm6%22,%22detail_E_R%22:%22detail_E_bm6%22,%22nose%22:%22nose_bm5%22,%22hat%22:%22hat_bmhairwrap%22,%22glasses%22:%22glasses_bm17%22}&colours={%22ff9866%22:16450293,%22ffcc99%22:5045420,%224f453e%22:4134404,%22926715%22:7455280,%2236a7e9%22:7916271,%226f4b4b%22:9603253}&body={%22body_type%22:3}&sex=1&outfit=889166&proportion=7&cropped=%22body%22&scale=1&style=4"/>
<img src="https://render.bitstrips.com//render/10217644/316830037_16_s4-v1.png?pd2={%22cranium%22:%22cranium_bm38%22,%22forehead%22:%22forehead_bm2%22,%22hair_back%22:%22hair_back_bm38%22,%22hair_front%22:%22hair_front_bm38%22,%22hairbottom%22:%22hairbottom_bm38%22,%22detail_L2_L%22:%22_blank%22,%22detail_L2_R%22:%22_blank%22,%22mouth%22:%22mouth_bm2%22,%22tongue%22:%22tongue_bm1_2%22,%22brow_L%22:%22brow_bm4%22,%22brow_R%22:%22brow_bm4%22,%22detail_T%22:%22detail_T_bm12%22,%22detail_L%22:%22detail_L_bm1%22,%22detail_R%22:%22detail_L_bm1%22,%22detail_E_L%22:%22detail_E_bm2%22,%22detail_E_R%22:%22detail_E_bm2%22,%22nose%22:%22nose_bm12%22,%22detail_E2_L%22:%22detail_E2_bm1%22,%22detail_E2_R%22:%22detail_E2_bm1%22,%22eyelid_L%22:%22eyelid_bm2_2%22,%22eyelid_R%22:%22eyelid_bm2_2%22,%22hat%22:%22hat_bmart7%22,%22glasses%22:%22glasses_bm4%22}&colours={%22ff9999%22:8659774,%22ff9866%22:7977513,%22ffcc99%22:2437679,%224f453e%22:4263197,%22926715%22:7753005,%2236a7e9%22:15558214,%22b88eb6%22:4899102}&body={%22body_type%22:0,%22breast_type%22:0}&sex=2&outfit=889211&proportion=0&cropped=%22body%22&scale=1&style=4"/>
</p>

---

## Using the program

Using Randmoji could not be any simpler! Simply fork the project from GitHub and run the only JavaScript file with Node. The program takes only one argument: the sex of the Bitmoji that you want to be generated. The options are `male` or `female`. This argument is needed because each sex has different attributes on the list that Randmoji polls from. Here's the program's syntax:

```shell
node randmoji.js <sex>
```
After running the script, it will output the link to your randomly generated Bitmoji! Simply copy and paste this image link into your browser or choice and enjoy!

---

## Understanding the Bitmoji API

In order to create a random Bitmoji, I had to understand how the API works. So here's what I figured out. You must provide a unique user-id. You can either use your own, or use someone else's since you are directly overriding the values associated with it. Look at the following example image URL:

```
https://render.bitstrips.com//render/10221787/316830037_16_s4-v1.png?pd2={%22cranium%22:%22cranium_bm35%22,%22forehead%22:%22forehead_bm1%22,%22hair_back%22:%22hair_back_blank%22,%22hair_front%22:%22hair_front_bm35%22,%22hairbottom%22:%22hairbottom_blank%22,%22beard%22:%22beard_bm4_1%22,%22stachin%22:%22stachin_bm1_1%22,%22stachout%22:%22stachout_bm1_1%22,%22mouth%22:%22mouth_bm3%22,%22tongue%22:%22tongue_bm1_1%22,%22brow_L%22:%22brow_bm3%22,%22brow_R%22:%22brow_bm3%22,%22detail_T%22:%22detail_T_bm14%22,%22detail_L%22:%22_blank%22,%22detail_R%22:%22_blank%22,%22detail_E_L%22:%22detail_E_bm7%22,%22detail_E_R%22:%22detail_E_bm7%22,%22nose%22:%22nose_bm15%22,%22hat%22:%22hat_bmfloppy%22,%22glasses%22:%22glasses_bm3d%22}&colours={%22ff9866%22:9476876,%22ffcc99%22:5988934,%224f453e%22:12795028,%22926715%22:2073019,%2236a7e9%22:921868,%226f4b4b%22:8626436}&body={%22body_type%22:1}&sex=1&outfit=889221&proportion=3&cropped=%22body%22&scale=1&style=4
```

This extremely large URL is composed of many small pieces of styling. Below will detail the basics of styling, and where you can find more information on styling your Bitmoji.
- `https://render.bitstrips.com//render/` is what lets the server know that you are rendering a custom avatar, not a Bitstrip comic. Comics are unable to be styled for some unknown reason.
- `10221787` is the unique comic ID. There are thousands of comics available in the [comics.json](json/comics.json) file. This ID is what determines what pose the Bitmoji will be in when rendered. Although all background clipart associated with the comic will not show, this still allows for thousands of possible poses.
- `316830037_16_s4-v1` is the unique user ID. Every registered Bitmoji user has one. This is different for a user's Bitmoji and Bitstrip avatars. The `_s4` signifies that its the Bitmoji version.
- `colours={%22ff9866%22:9476876,%22ffcc99%22:5988934,%224f453e%22:12795028,%22926715%22:2073019,%2236a7e9%22:921868,%226f4b4b%22:8626436}` is responsible for changing the colors of different parts of the Bitmoji. Every color contained in the object has a key and value. The key is what determines what is being colored, and the value is the color itself. Bitmoji's color values are in decimal (base 10), so don't use hexadecimal or the server will throw an error.
- `pd2={%22cranium%22:%22cranium_bm35%22,%22forehead%22:%22forehead_bm1%22,%22hair_back%22:%22hair_back_blank%22,%22hair_front%22:%22hair_front_bm35%22,%22hairbottom%22:%22hairbottom_blank%22,%22beard%22:%22beard_bm4_1%22,%22stachin%22:%22stachin_bm1_1%22,%22stachout%22:%22stachout_bm1_1%22,%22mouth%22:%22mouth_bm3%22,%22tongue%22:%22tongue_bm1_1%22,%22brow_L%22:%22brow_bm3%22,%22brow_R%22:%22brow_bm3%22,%22detail_T%22:%22detail_T_bm14%22,%22detail_L%22:%22_blank%22,%22detail_R%22:%22_blank%22,%22detail_E_L%22:%22detail_E_bm7%22,%22detail_E_R%22:%22detail_E_bm7%22,%22nose%22:%22nose_bm15%22,%22hat%22:%22hat_bmfloppy%22,%22glasses%22:%22glasses_bm3d%22}` is what determines each and every unique property. Just like the colors, every item has a key and value pair. All possible options are outlined in the [bitmoji.json](json/bitmoji.json) file. Use this as a guide on sending a custom query.
- `body={"body_type":1}` is what sets the physical size of the Bitmoji (such as weight, and breast size on female avatars). These values are also listed in the JSON file.
- `cropped="body"` sets the avatar to crop all extra space to the body. The edges of the images will be as tight around the avatar as possible. The only other possible options are `head` or empty.
- `outfit=889221` sets the outfit.
- `scale=1` changes the resolution of the rendered avatar. Higher values are better resolutions.
- `style=4` This does not directly affect anything, but is associated with the style of the Bitmoji. Just like `_s4` in the unique ID.
- `sex=1` signifies the Bitmoji's sex. `1` is for male, `2` is for female.
- `proportion=3` determines the face/head shape.
- There are other options that dtermine what the image will look like such as `head_rotation=` and `body_rotation=`. These parameters take a numeric value and cause the image to rotate that specific part of the avatar.

Not all of these values need to be used or provided. Simply add any parameter that you desire. Finally, the above URL provided as an example would render the following image:
<p align="center">
<img src="https://render.bitstrips.com//render/10221787/316830037_16_s4-v1.png?pd2={%22cranium%22:%22cranium_bm35%22,%22forehead%22:%22forehead_bm1%22,%22hair_back%22:%22hair_back_blank%22,%22hair_front%22:%22hair_front_bm35%22,%22hairbottom%22:%22hairbottom_blank%22,%22beard%22:%22beard_bm4_1%22,%22stachin%22:%22stachin_bm1_1%22,%22stachout%22:%22stachout_bm1_1%22,%22mouth%22:%22mouth_bm3%22,%22tongue%22:%22tongue_bm1_1%22,%22brow_L%22:%22brow_bm3%22,%22brow_R%22:%22brow_bm3%22,%22detail_T%22:%22detail_T_bm14%22,%22detail_L%22:%22_blank%22,%22detail_R%22:%22_blank%22,%22detail_E_L%22:%22detail_E_bm7%22,%22detail_E_R%22:%22detail_E_bm7%22,%22nose%22:%22nose_bm15%22,%22hat%22:%22hat_bmfloppy%22,%22glasses%22:%22glasses_bm3d%22}&colours={%22ff9866%22:9476876,%22ffcc99%22:5988934,%224f453e%22:12795028,%22926715%22:2073019,%2236a7e9%22:921868,%226f4b4b%22:8626436}&body={%22body_type%22:1}&sex=1&outfit=889221&proportion=3&cropped=%22body%22&scale=1&style=4"/>
</p>

---

## Product disclaimer

This code is in no way affiliated with, authorized, maintained, sponsored or endorsed by Bitmoji or any of its affiliates or subsidiaries. This is an independent and unofficial product. Use at your own risk.
