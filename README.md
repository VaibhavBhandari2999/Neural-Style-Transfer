# Neural-Style-Transfer

Neural style transfer is an optimization technique used to take three images, a content image, a style reference image (such as an artwork by a famous painter), and the input image you want to style — and blend them together such that the input image is transformed to look like the content image, but “painted” in the style of the style image.

We use the VGG19 model for this implementation. VGG19 is easily downloadable from keras.

Neural style transfer uses a pretrained convolution neural network. Then to define a loss function which blends two images seamlessly to create visually appealing art, NST defines the following inputs:
A content image (c) — the image we want to transfer a style to
A style image (s) — the image we want to transfer the style from
An input (generated) image (g) — the image that contains the final result (the only trainable variable)
The architecture of the model as well as how the loss is computed is shown below. 

![1_ZgW520SZr1QkGoFd3xqYMw](https://user-images.githubusercontent.com/30387574/83442587-06726080-a466-11ea-8b8f-d0f0ccdddeaf.jpeg)

<h3>Output</h3>
I have used an image of Andrew NG as the <b>Content Image</b><br>
I have used a cubic piece of art by Picasso as the <b>Style Image</b><br>
<br>
The generated image is essentialy a mix of both, with Andrew NG drawn in the style of Picasso.

![content_2](https://user-images.githubusercontent.com/30387574/83443189-f60eb580-a466-11ea-8fa7-0f443eef8886.jpg)<h1> +</h1> ![style_3](https://user-images.githubusercontent.com/30387574/83443229-0aeb4900-a467-11ea-9379-a9d14147b2af.jpg) <h1>=</h1> ![xyz](https://user-images.githubusercontent.com/30387574/83443267-18a0ce80-a467-11ea-826e-d9a8fd62a665.png)
