<h1>KATO, the Klipper Augmented Text Optimizer</h1>

As the ultimate macro for styling text, KATO is a versatile tool that allows you to add style and flair to your console output text in Mainsail and Fluidd. It offers a wide range of customization options to make your text pop in anyway you can imagine!![Screenshot 2023-09-07 163519](https://github.com/TmRxJD/Klipper_Augmented_Text_Optimizer/assets/141893411/1fa3f0f4-a7e7-4bf2-bc3d-d9357ecd34de)


<h2>Features:</h2>

Text Coloring: Choose from a variety of text colors to make your text stand out.

Background Color: Add background color to your text for contrast.

Font Size: Adjust the font size to make your text bigger or smaller.

Font Style: Customize the font with bold and italic options.

Text Decoration: Apply underline or strike-through styles to your text.

Line Color: Specify the color for text decorations.

Opacity: Control the opacity of your text to make it more or less transparent.

Borders: Add borders around your text with customizable border color and size, as well as type, such as solid, dashed, inset, etc.

Font Selection: Choose from a variety of fonts like Arial, Calibri, and more.

Palette Selection: Save your favorite values within the macro to call later as a palette. Example: "text_styler palette=2" You can also still customize individual options within each palette.

Randomization: The default behavior will pick a random option from the available selections, but you can disable this and have it cycle instead with "randomize=false"

Style by the Word or by the Letters: by default the macro will alter every character, but you can disable this and have it do entire words instead with "by_word=true"

<h3>Usage:</h3>

The Text Styler Macro supports the ability to add multiple options, and it will cycle through all that are available, allowing you to create dynamic and visually appealing text. You can specify multiple values for each style parameter, and the macro will apply them sequentially. So setting the colors to red and blue will alternate between red and blue. You can add as many color options as you want. 

<h4>Example Syntax</h4>

You can pass text from other macros into this one to output the text, or you can play with modifying text directly in the console. 

Type into your console: "text_styler by_word=true(false by default) font_sizes=option1,option2 bg_colors=option1,option2 text_colors=option1,option2 opacities=option1,option2 line=underline,strike,none line_colors=option1,option2 fonts=option1,option2 bold=bold,none italic=italic,none border_colors=option1,option2 glow_colors=option1,option2 glow_size=option1,option2 randomize=false(true by default) message="your message here""

Example: "text_styler by_word=true font_sizes=25 bg_colors=black,blue text_colors=blue,black opacities=1,0.25 line=underline line_colors=purple fonts=gothic,arial bold=bold, italic=none,italic border_colors=blue,black glow_colors=yellow glow_size=15 message="Enjoy using the text styler!""

Make sure there is no space between options, they should only be separated by a comma, spaces should separate the different parameters, not the values within then. Case does not matter. 

It is a best practice to use css span tag names like "primary" and "error" for your text color options to ensure better readibility with themes, but you can set these however you wish. You cam only use actual color names with background colors. 
