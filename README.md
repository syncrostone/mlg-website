# MLG website

MS teams channel: new MLG website

If you have any problems, please bring it up the MS teams channel. Others might be having the same issue and they may be able to help.

Contact: Marton Havasi (mh740@cam.ac.uk)

# FAQ

## How can I update my profile?

1. Make sure you are part of the cambridge-mlg github group `github.com/cambridge-mlg`.

2. Clone the repository for the website

```
git clone https://github.com/cambridge-mlg/mlg-website.git
```

3. Add your profile by editing `mlg-website/content/members/_index.md`

Here is the template. Make sure to set a unique name for your profile picture (this will be relevant later):

```
{{< figure src="/images/<yourname>.jpg" class="profile-image">}}

### <Your Name>

This is some text that describes your background and/or research interests. Please write at least a 3-4 of sentences. You can also link your website/twitter if you have one like this: [My website](https://www.<your_website>.com) [My Twitter](https://twitter.com/<twitter_profilename>)
```

4. Add your profile picture under `mlg-website/static/images`. Make sure that the filename matches the one you used in step 3.

5. Once you are happy with the text and the image, commit it:

```
git add static/images/<yourname>.jpg
git commit -m '<Your Name> profile'
git push
```

6. The changes only go into effect when some runs the deployment script. Please don't run it yourself, contact the person maintaining the website to do it. The preferred way is to post in the MS teams channel and ask someone to run it.

## How can I make a fancy profile?

Here are some formatting instructions you can use: https://sourceforge.net/p/hugo-generator/wiki/markdown_syntax/

## I am not familiar with git, I need help

Post in the MS teams channel or contact the person maintaining the website.

## I have some recommendations for stylistic changes

When deploying the website, we prioritized speed over looks to make sure that our prospective PhD applicants have up-to-date info. We first want to make sure that the website is functional, then we will make it look good. If you have any recommendations, please post them in the MS teams channel.

## How do I run the deployment script? (advanced)

1. Install hugo 

```
brew install hugo
# or
port install hugo
```

To verify your new install:

```
hugo version
```

This tutorial may be helpful: https://gohugo.io/getting-started/quick-start/

2. `./deploy.sh`

This tutorial may be helpful: https://gohugo.io/hosting-and-deployment/hosting-on-github/




