# 0x0B. Implement a design with bootstrap


In this project, you will implement 3 web pages with Bootstrap.
You will use all HTML/CSS/Accessibility/Responsive design/Bootstrap knowledges that you learned previously. 
You won’t have a lot of instruction, you are free to implement it the way that you want - the objective is simple: Have fully functional web pages that look the same as the designer file.
Here the final result:
<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3c71cc99d2fc1c12a3d3.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=84e4be49002003bf0a2d8772d35faaffd19563c7943104ecd7a6f66d9f2deb28" alt="" style="">
This webpage has been designed by Nicolas Philippot, UI/UX designer. 
You can find final screens [here](https://intranet-projects-files.s3.amazonaws.com/holbertonschool-webstack/623/Archive.zip)
### Requirements
  + You have to use Bootstrap
  + Your `styles.css` must be as small as you can - **you must use as much as you can Bootstrap classes**

### Imports
For this project, you will need: fonts from Google, JQuery, Bootstrap CSS/JS

```
<link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Coiny&display=swap" rel="stylesheet">

<script src="https://code.jquery.com/jquery-3.4.1.min.js" integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>

<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
```


## 0. Read and be familiar with Figma
Create an account in <a href="/rltoken/0OS4ME4Kjnw0I82IVkkoSw" title="Figma" target="_blank">Figma</a> and open these files:

Create an account in [Figma](https://intranet.hbtn.io/rltoken/0OS4ME4Kjnw0I82IVkkoSw) and open these files:
  + [Homepage](https://intranet.hbtn.io/rltoken/RLej4Ua6W3EmDh7UCwGTzQ) - [fig file](https://intranet.hbtn.io/rltoken/1ZTxYF-usvxpIjj44YYcyw)
  + [Pricing](https://intranet.hbtn.io/rltoken/xQCL77_ePGWntUAe4T7ebQ) - [fig file](https://intranet.hbtn.io/rltoken/AdJ6ZyZrG90gRNAI5bt_lA)
  + [Courses](https://intranet.hbtn.io/rltoken/__3w9ryapSUAwMaAYYS6ZA) - [fig file](https://intranet.hbtn.io/rltoken/1JL-gCkfJ5Hqb0Sf2lmymw)

And “Duplicate to your Drafts” to have access to all design details.

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/559ad8d43fb61e310e2b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=7d0bfa92c953793529698d6b060c69100b7c1aa27947afa2b77fcbeb82f889b3" alt="" style="">

Important notes with Figma:
  + if your computer doesn’t have missing fonts, you can find them here: [source-sans-pro](https://intranet.hbtn.io/rltoken/4uQkoVbAjr7lRVqSVCWBcw) and [Spin-Cycle-OT](https://intranet.hbtn.io/rltoken/5HnXzrMbtVKLCScrdy4CIg)
  + some values are in float - feel free to round them
  + “Be pixel perfect” - yes! but mainly make sure colors, size and position are correct. <span style="background-color: #C271FF">#C271FF</span> is not <span style="background-color: purple">purple</span>.

For this task, please write an amazing `README.md`

**Interactions note:**
  + Web pages must switch to the tablet version when the screen width is 768px
  + Web pages must switch to the mobile version when the screen width is 576px
  + button hover/active: `opacity: 0.9`


## 1. Header first
Let’s start by the Homepage: <strong>create the header/hero piece</strong>

Let’s start by the Homepage: **create the header/hero piece**

Here an archive of all assets needed (for the entire project):
  + [images_images.zip](https://holbertonintranet.s3.amazonaws.com/uploads/misc/2020/3/e62e701b6ce0374555e9.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=345600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=001d7ee25d2eeb155f29f8019db697f60ec9fdb3cf03f829480036812affa0e6)
  + [holberton_school-icon.zip](https://holbertonintranet.s3.amazonaws.com/uploads/misc/2020/3/7159d988278de54d859d.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=345600&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=686fa26a84fdeba3831e2d2075d54a8d346be00501c18c6b1c4aa18c7a9f7490)

**Desktop:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/13572c3773e26651761e8b4a74b3383300ed9563.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=e7b00db280151063b69e33f47f5f4acce9a2becb434e05e90b44a2da7ab82f20" alt="" style="">

**Mobile:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/8854d68a957ef7dc2315.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=34e4764071eeb64e38631b267f6d46c2603c6559d59a6f99e85f1d36212ba2c2" alt="" style="">


## 2. Carousel of quotes
<strong>Create the section “Carousel of quotes”</strong>

**Create the section “Carousel of quotes”**

By using a Carousel component of Bootstrap, create this Carousel of quotes. 

You can have for the moment one quote or twice the same for testing (like example below)

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/8455560f9ac188658195.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=e39cd4f88f03168847621c93e49a8166329f440997a60f9ab53538a8cabd1c99" alt="" style="">


## 3. Popular videos
<strong>Create the section “Most popular tutorials”</strong>

**Create the section “Most popular tutorials”**

By using a Carousel component of Bootstrap, create this Carousel of video cards. 

**Reminder:**
  + Desktop: 4 cards
  + Tablet: 2 cards
  + Mobile: 1 card

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/4b610dc2d2cc17ceb2f7.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=b8f0f216a90ef47406d0f15fa79768390c68a64a24e428c1529fe320f6d7f350" alt="" style="">


## 4. Row of smiles
<strong>Create the section “Free membership”</strong>

**Create the section “Free membership”**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/970efd54768b693bbfac.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=247e70222ff9356a8dff162f6192b8359e84c8fdd37e5b87cd1893ba674114ca" alt="" style="">


## 5. Latest videos
<strong>Create the section “Latest videos”</strong>

**Create the section “Latest videos”**

Copy the block “Most popular tutorials” to “Latest videos”


## 6. ... and the footer!
<strong>Create the footer</strong>

**Create the footer**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/739d7cc60098e7ff8f25.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=2211e675560ae4be7e090e0a586ce055580dcf9417b05f7f783d4a888f13d552" alt="" style="">


## 7. Pricing - header
Now, let’s do the pricing page: <strong>create the header/hero piece</strong>

Now, let’s do the pricing page: **create the header/hero piece**

The mobile version must be the same as the Homepage - it’s time to reuse code!

**Desktop:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/ccd30a4d80a990b96740.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=589989c99f7401eda8b5a123e9df38fe04c04a45ad2b2b0a59b42df553945a49" alt="" style="">


## 8. Prices grid
<strong>Create the prices grid</strong>

**Create the prices grid**

**Desktop:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/0ac3872946a0014e4f99.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=93e5a596b597307191150ffabfe8d54c1f12431888df0535b36dc2a7763c1a98" alt="" style="">

**Mobile:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/edea8172b9cc0a867237.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=dcbd520274c4ec1c8e517de42b5a0264ea37f05550ce68775053d400d8725cda" alt="" style="">


## 9. Quotes section
Same as the Homepage, <strong>create the Carousel of quotes</strong>

Same as the Homepage, **create the Carousel of quotes**


## 10. FAQ
<strong>Create the FAQ grid</strong>

**Create the FAQ grid**

**Desktop:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/db8f90e37593a29c1ab6.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=30cb1167bc95e0775b83567ae876e2a3149d7abf1ee3298b68f47c1c0a9dd762" alt="" style="">

**Mobile:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/eaeb117d40690a451c7b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=fa5e1151292810f0b00e799ca80d0d77b25eed842077438e4dff84d14294b056" alt="" style="">


## 11. Close the page with a footer
Same as Homepage, <strong>create the footer</strong>

Same as Homepage, **create the footer**


## 12. Courses - header
Now, let’s do the courses page: <strong>create the header/hero piece</strong>

Now, let’s do the courses page: **create the header/hero piece**

The mobile version must be the same as the Homepage - it’s time to reuse code!

**Desktop:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/a5ba265af5dd643ad942.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=76bee27f77e050b62101921fe378c56139090c4a63ecab440649295ad0de5986" alt="" style="">


## 13. Search filters
<strong>Create the search filters section</strong>

**Create the search filters section**

Dropdown is a nice way to create filters.

For the selected/placeholder value of both dropdown, no need to have dynamic value - static content is totally ok.

**Desktop:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/98c0564e59ec5620990e.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=61491bb4a4a29cf8db3f865cdc6a2cd927e7b3e30e50f18bf39958772e402b8a" alt="" style="">

**Tablet/Mobile:**

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3627550eccca7958d390.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=bc8af9627082f9504e1eeeb75ece5eac9a701e154fffdf970277b3e258e2e731" alt="" style="">


## 14. List of result
<strong>Create the result section of courses</strong>

**Create the result section of courses**

You can reuse the same cell for testing. 
Don’t forget to test with odd and even number of cells.

<img src="https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/76b2074f3f6bbd25cdb9.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOUWMNL5ANN%2F20210908%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210908T131236Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=3519dd0883d082c9694b9887e38fdf519f1d94b07c575a89b795bab94ef4a418" alt="" style="">


## 15. Close the page with a footer
Same as Homepage and Pricing page, <strong>create the footer</strong>

Same as Homepage and Pricing page, **create the footer**
