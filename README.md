# Stage_D_Quiz
Different parameters were used to acquire the best mean Fbeta in this project.
The first model used was the Vgg16, but then i realized i needed to use a better model.
i ended up using the Resnet model
I couldn't use flow_from_directory because of the error of "finding 0 images belonging to 0 Classes", so i ended up using flow_from_dataframe.
My initial optimizer was Adamax, but it wasn't giving me good Fbeta, the i changed to Adam, and i had a better result.
With Learning rate of 0.001, my highest Fbeta score was 0.8, but when i changed to 0.0001, it then increased to 0.91442.
My initial threshold was 0.5, but then changing it to 0.2 inorder to have more true_positive, my Fbeta score also increased a little.
The last change was on the epoch used, initial epoch was 10, and then later changed to 20, wihich gave me val_fbeta of 0.91720.

Thank you for reading
