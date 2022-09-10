# Duplicat_image_Detection
A solution to find Duplicate Images on your system  or Any images  downloaded via urls .

Here we are fetching urls from an input Csv and downloading Each image from url of one column and comparing with all images given in next column one by one.


Solution We are using To find duplicate is:


##    Hashing

#### Simply said, Hashing is the transformation of any data into a usually shorter fixed-length value or key that represents the original string.

Just as we have unique Fingerprints, Hashes are unique for any particular data. There are lots of Hashing Algorithms out there which cater to specific needs.


####### Since it’s ability to generate unique fingerprints, we can use Hashing to find duplicates, since similar images will have the same fingerprints.

In order to compare images to one another, we need to somehow translate them into comparable, computer-readable i. e. numeric data. Those of you that are familiar with machine learning and computer vision may already know that images can be translated into matrices, or more precisely into a tensor. A tensor is a container which can hold data in N dimensions. A matrix therefore is a 2-dimensional tensor.



#### But there’s a small catch

Most Hashing Algorithms will work for Finding Duplicates but very few will be able to find similar Images. Why? Since these algorithms produce big changes in the hash even though if there is a small change in data.
What do we do then?

We need to use a Hashing Algorithm specifically developed for Images i.e Average Hashing. This algorithm helps to solve the issue by creating smaller differences in hashes for similar pictures.






Average Hashing

Average Hashing is a very powerful algorithm specifically made for images.

It works in these specific steps:

    * Reduce the size of the image (For better performance and removing high frequencies.)
    * Convert to GrayScale.
    * Compute the mean pixel value of the entire Image.
    * Use the mean as a threshold to convert the entire image into 0 or 1 bits.
    * Construct the Hash.
    
    
    
![1 DdtUafvmHdkqPQifXLhJ4w](https://user-images.githubusercontent.com/92270337/189487382-d01931bd-92f0-47d8-a491-945af9b63a5d.png)
