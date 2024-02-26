# Currencies-Price-prediction

#This code is to get data of last 30 days from Investing,com and apply Time series ARIMA to it to predect the future pr



w=pred()
gbpusdData=w.getData('https://www.investing.com/currencies/gbp-usd-historical-data')

print(gbpusdData)

      


warnings.filterwarnings("ignore")
forcast=w.estim(gbpusdData)


![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/05fdfda1-7c53-48f6-9226-4ee2b06bfca3)

w=pred()
eurusdData=w.getData('https://www.investing.com/currencies/eur-usd-historical-data')

print(eurusdData)


warnings.filterwarnings("ignore")
forcast=w.estim(eurusdData)

![download](https://github.com/Fadhaa/Currencies-Price-prediction/assets/18240431/b1aea97d-b0cf-461d-8702-92ca9643aacc)


print("The mse of the (Low, High) forcasting is")
print(forcast)[Uploading Code for forecasting currency-crosses from investing - JupyFrom: <Saved by Blink>
Snapshot-Content-Location: http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#
Subject: Code for forecasting currency-crosses from investing - Jupyter Notebook
Date: Tue, 27 Feb 2024 00:40:36 +0300
MIME-Version: 1.0
Content-Type: multipart/related;
	type="text/html";
	boundary="----MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----"


------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/html
Content-ID: <frame-FBEE8D5854DA284EFC3A5620D5AED36D@mhtml.blink>
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#

<!DOCTYPE html><html lang=3D"en-us"><head><meta http-equiv=3D"Content-Type"=
 content=3D"text/html; charset=3DUTF-8"><link rel=3D"stylesheet" type=3D"te=
xt/css" href=3D"cid:css-cf0de846-b81b-415b-b4ae-0efe32fe6a1f@mhtml.blink" /=
><link rel=3D"stylesheet" type=3D"text/css" href=3D"cid:css-c3982157-b0ef-4=
9d1-b6c6-bf731d1e50a4@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/=
css" href=3D"cid:css-b5b5bf9d-9255-45e7-bc73-7909123caf80@mhtml.blink" /><l=
ink rel=3D"stylesheet" type=3D"text/css" href=3D"cid:css-d5fa4ba8-dd42-41b1=
-a3f6-e37c4ae43185@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css=
" href=3D"cid:css-75e0ea17-5bb2-43a3-9c86-5539cd4d9e14@mhtml.blink" /><link=
 rel=3D"stylesheet" type=3D"text/css" href=3D"cid:css-96a39898-bcc9-48ae-9d=
83-74b6eb3afb0d@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" h=
ref=3D"cid:css-57dffdf9-e0fd-4707-a914-03051e14c18b@mhtml.blink" /><link re=
l=3D"stylesheet" type=3D"text/css" href=3D"cid:css-46264988-c362-4058-a17a-=
20d3ea3c46ca@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-0bfb7d94-ed8f-4684-ac25-c9e5b1abb8f3@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-854fd570-7fde-4c96-a903-9=
8e468bbaec8@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-7fce1f8c-a4bc-4861-a819-2a17277aa1bb@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-54248245-f784-467f-8808-b=
ac75ad7fe78@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-3ba88621-bb13-4404-9787-bdcb6456eb83@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-444b85d2-0450-4409-a3de-3=
e2c0d9f1571@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-4ba1a7b4-c904-4133-892e-2a4002beb30b@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-492c6891-d580-4652-90ff-0=
0c3d071f793@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-a8783c95-b9ef-4884-b3d4-b921582b750e@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-998870eb-cf54-46b5-a917-c=
9493e8ba448@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-762778e4-e802-4417-8169-e36bff4175c8@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-35a3899a-3a68-4437-a357-1=
87824ba8916@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-b9e99216-e19e-4d0f-941f-f0e668c88f66@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-22f22da9-a8a4-4cef-bd16-6=
0fd40b7da6c@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-cf5c9e11-0496-4d3c-b88d-a86b837bca1d@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-cbc856b7-4060-4ee6-97c7-f=
0fed95caf41@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-ae5dcdd6-9045-4819-b495-d9566b7acc94@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-e5247429-5cc2-4e23-bd91-8=
acda443531f@mhtml.blink" /><link rel=3D"stylesheet" type=3D"text/css" href=
=3D"cid:css-032bdaa1-972d-4a50-8866-40e7a05b517c@mhtml.blink" /><link rel=
=3D"stylesheet" type=3D"text/css" href=3D"cid:css-89c58381-a5d3-49a2-96b6-7=
58f3f064c43@mhtml.blink" />
   =20

    <title>Code for forecasting currency-crosses from investing - Jupyter N=
otebook</title>
   =20
    <meta http-equiv=3D"X-UA-Compatible" content=3D"IE=3Dedge">
    <link rel=3D"stylesheet" href=3D"http://localhost:8890/static/component=
s/jquery-ui/dist/themes/smoothness/jquery-ui.min.css?v=3D32f9dcde0cd9843f2b=
66d34c1c9928b59a5d7ef007ba7a6a6a790b3e78f7857a698444d7a716dfaf8fa834c3b3175=
efd258bbc07cfc4aabb86769b07e5f358c3" type=3D"text/css">
    <link rel=3D"stylesheet" href=3D"http://localhost:8890/static/component=
s/jquery-typeahead/dist/jquery.typeahead.min.css?v=3D5edf53bf6bb9c3b1ddafd8=
594825a7e2ed621f19423e569c985162742f63911c09eba2c529f8fb47aebf27fafdfe287d5=
63347f58c1126b278189a18871b6a9a" type=3D"text/css">
    <meta name=3D"viewport" content=3D"width=3Ddevice-width, initial-scale=
=3D1.0">
   =20
   =20






<link rel=3D"stylesheet" href=3D"http://localhost:8890/static/components/bo=
otstrap-tour/build/css/bootstrap-tour.min.css?v=3D95c93e52db61ab29625defe55=
361384ce6776a7d303b97da5a73fef5ddf8e391a6223599a0b58669476bd71645a4f0022df0=
517c88b0c05df80ba465e36f5417" type=3D"text/css">
<link rel=3D"stylesheet" href=3D"http://localhost:8890/static/components/co=
demirror/lib/codemirror.css?v=3Da545ad5e21a51420a7cb40234688eef087a5cf3798f=
64d7750291a8be0e9c760b8a1c9cbbbdcaa6470f2f385caa59e816f2640f609d29147f4762e=
27f69709e6">


    <link rel=3D"stylesheet" href=3D"http://localhost:8890/static/style/sty=
le.min.css?v=3De1ab1c38b672063a6541baf468c83345cd0f509729783ec9b7ccb6407300=
4f5f056110c82c28aefbf3dbf32e0e040f05b8f0420bc411b669ed3d4f07511812ca" type=
=3D"text/css">
   =20

<link rel=3D"stylesheet" href=3D"http://localhost:8890/static/notebook/css/=
override.css?v=3D16733f6ba5f2224692fe4e654f3cbb2e3cae82f1df06ca53aa1cb88b14=
7465f16c968c0898e2b0203a7ad3a469f82b959e26bb4b27b790f7f364c4336449b0aa" typ=
e=3D"text/css">



    <link rel=3D"stylesheet" href=3D"http://localhost:8890/custom/custom.cs=
s" type=3D"text/css">
   =20
   =20
   =20
   =20
   =20
   =20

   =20
   =20

<link id=3D"favicon" type=3D"image/x-icon" rel=3D"shortcut icon" href=3D"ht=
tp://localhost:8890/static/base/images/favicon-notebook.ico"></head>

<body class=3D"notebook_app command_mode" data-jupyter-api-token=3D"82ca588=
0f84f70681a5e735e03f85ff4c3e0cddfda89ae71" data-base-url=3D"/" data-ws-url=
=3D"" data-notebook-name=3D"Untitled4.ipynb" data-notebook-path=3D"Untitled=
4.ipynb" dir=3D"ltr"><div style=3D"visibility: hidden; overflow: hidden; po=
sition: absolute; top: 0px; height: 1px; width: auto; padding: 0px; border:=
 0px; margin: 0px; text-align: left; text-indent: 0px; text-transform: none=
; line-height: normal; letter-spacing: normal; word-spacing: normal;"><div =
id=3D"MathJax_Hidden"></div></div><div id=3D"MathJax_Message" style=3D"disp=
lay: none;"></div>



<div id=3D"header" role=3D"navigation" aria-label=3D"Top Menu" style=3D"dis=
play: block;">
  <div id=3D"newsId" style=3D"display: none;">
   =20
    <div class=3D"alert alert-info" role=3D"alert">
      <div style=3D"display: flex">
        <div>
          <span class=3D"label label-warning">UPDATE</span>
          Read <a href=3D"https://jupyter-notebook.readthedocs.io/en/latest=
/migrate_to_notebook7.html" style=3D"text-decoration: underline;" target=3D=
"_blank">the migration plan</a> to Notebook 7 to learn about the new featur=
es and the actions to take if you are using extensions
          -
          Please note that updating to Notebook 7 might break some of your =
extensions.
        </div>
        <div style=3D"margin-left: auto;">
          <a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasti=
ng%20currency-crosses%20from%20investing.com%20">
            <button type=3D"button" class=3D"btn btn-default btn-xs" id=3D"=
dontShowId">
              Don't show anymore
            </button>
          </a>
        </div>
      </div>
    </div>
   =20
  </div>
  <div id=3D"header-container" class=3D"container">
  <div id=3D"ipython_notebook" class=3D"nav navbar-brand"><a href=3D"http:/=
/localhost:8890/tree?token=3D82ca5880f84f70681a5e735e03f85ff4c3e0cddfda89ae=
71" title=3D"dashboard">
      <img src=3D"http://localhost:8890/static/base/images/logo.png?v=3Da2a=
176ee3cee251ffddf5fa21fe8e43727a9e5f87a06f9c91ad7b776d9e9d3d5e0159c16cc188a=
3965e00375fb4bc336c16067c688f5040c0c2d4bfdb852a9e4" alt=3D"Jupyter Notebook=
">
  </a></div>

 =20


<span id=3D"save_widget" class=3D"save_widget">
    <span id=3D"notebook_name" class=3D"filename">Code for forecasting curr=
ency-crosses from investing</span>
    <span class=3D"checkpoint_status" title=3D"Tue, Feb 27, 2024 12:18 AM">=
Last Checkpoint: 21 minutes ago</span>
    <span class=3D"autosave_status">(autosaved)</span>
</span>


 =20

<span id=3D"kernel_logo_widget">
 =20
  <img class=3D"current_kernel_logo" alt=3D"Current Kernel Logo" src=3D"htt=
p://localhost:8890/kernelspecs/python3/logo-64x64.png" title=3D"Python 3 (i=
pykernel)" style=3D"display: inline;">
 =20
</span>


 =20
 =20
 =20
 =20

    <span id=3D"login_widget">
     =20
        <button id=3D"logout" class=3D"btn btn-sm navbar-btn">Logout</butto=
n>
     =20
    </span>

 =20

 =20
 =20
  </div>
  <div class=3D"header-bar"></div>

 =20
<div id=3D"menubar-container" class=3D"container">
<div id=3D"menubar">
    <div id=3D"menus" class=3D"navbar navbar-default" role=3D"navigation">
        <div class=3D"container-fluid">
            <button type=3D"button" class=3D"btn btn-default navbar-btn nav=
bar-toggle" data-toggle=3D"collapse" data-target=3D".navbar-collapse">
              <i class=3D"fa fa-bars"></i>
              <span class=3D"navbar-text">Menu</span>
            </button>
            <p id=3D"kernel_indicator" class=3D"navbar-text indicator_area"=
>
              <span class=3D"kernel_indicator_name">Python 3 (ipykernel)</s=
pan>
              <i id=3D"kernel_indicator_icon" class=3D"kernel_idle_icon" ti=
tle=3D"Kernel Idle"></i>
            </p>
            <i id=3D"readonly-indicator" class=3D"navbar-text" title=3D"Thi=
s notebook is read-only" style=3D"display: none;">
                <span class=3D"fa-stack">
                    <i class=3D"fa fa-save fa-stack-1x"></i>
                    <i class=3D"fa fa-ban fa-stack-2x text-danger"></i>
                </span>
            </i>
            <i id=3D"modal_indicator" class=3D"navbar-text modal_indicator"=
 title=3D"Command Mode"></i>
            <span id=3D"notification_area"><div id=3D"notification_kernel" =
class=3D"notification_widget btn btn-xs navbar-btn undefined info" style=3D=
"display: none;"><span></span></div><div id=3D"notification_notebook" class=
=3D"notification_widget btn btn-xs navbar-btn" style=3D"display: none;"><sp=
an></span></div><div id=3D"notification_trusted" class=3D"notification_widg=
et btn btn-xs navbar-btn" disabled=3D"disabled" style=3D"cursor: help;"><sp=
an title=3D"Javascript enabled for notebook display">Trusted</span></div><d=
iv id=3D"notification_widgets" class=3D"notification_widget btn btn-xs navb=
ar-btn" style=3D"display: none;"><span></span></div></span>
            <div class=3D"navbar-collapse collapse">
              <ul class=3D"nav navbar-nav">
                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" class=3D"dropdown-toggle" id=3D"filelink" data-toggle=3D"dropdown" aria=
-haspopup=3D"true" aria-controls=3D"file_menu" aria-expanded=3D"false">File=
</a>
                    <ul id=3D"file_menu" class=3D"dropdown-menu" role=3D"me=
nu" aria-labelledby=3D"filelink">
                        <li id=3D"new_notebook" class=3D"menu_focus_highlig=
ht dropdown dropdown-submenu" role=3D"none">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" class=3D"dropdown=
-toggle" data-toggle=3D"dropdown">New Notebook<span class=3D"sr-only">Dropd=
own</span></a>
                            <ul class=3D"dropdown-menu" id=3D"menu-new-note=
book-submenu" role=3D"menu">
                            <li id=3D"new-notebook-submenu-python3"><a href=
=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-cro=
sses%20from%20investing.com%20#">Python 3 (ipykernel)</a></li></ul>
                        </li>
                        <li id=3D"open_notebook" role=3D"none" title=3D"Ope=
ns a new window with the Dashboard view">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Open...</a></li>
                        <!-- <hr/> -->
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"copy_notebook" role=3D"none" title=3D"Ope=
n a copy of this notebook's contents and start a new kernel">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Make a Copy...</a></li>
                        <li id=3D"save_notebook_as" role=3D"none" title=3D"=
Save a copy of the notebook's contents and start a new kernel">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Save as...</a></li>
                        <li id=3D"rename_notebook" role=3D"none"><a href=3D=
"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosse=
s%20from%20investing.com%20#" role=3D"menuitem">Rename...</a></li>
                        <li id=3D"save_checkpoint" role=3D"none"><a href=3D=
"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosse=
s%20from%20investing.com%20#" role=3D"menuitem" class=3D"menu-shortcut-cont=
ainer"><span class=3D"action">Save and Checkpoint</span><span class=3D"kb">=
<kbd>Ctrl-S</kbd></span></a></li>
                        <!-- <hr/> -->
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"restore_checkpoint" class=3D"menu_focus_h=
ighlight dropdown-submenu" role=3D"none"><a href=3D"http://localhost:8890/n=
otebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com=
%20#" role=3D"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" clas=
s=3D"dropdown-toggle" data-toggle=3D"dropdown">Revert to Checkpoint<span cl=
ass=3D"sr-only">Dropdown</span></a>
                          <ul class=3D"dropdown-menu"><li><a href=3D"http:/=
/localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20fro=
m%20investing.com%20#">Tuesday, February 27, 2024 12:18 AM</a></li></ul>
                        </li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"print_preview" role=3D"none"><a href=3D"h=
ttp://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%=
20from%20investing.com%20#" role=3D"menuitem">Print Preview</a></li>
                        <li class=3D"dropdown-submenu menu_focus_highlight"=
 role=3D"none"><a href=3D"http://localhost:8890/notebooks/Code%20for%20fore=
casting%20currency-crosses%20from%20investing.com%20#" role=3D"menuitem" ar=
ia-haspopup=3D"true" aria-expanded=3D"false" class=3D"dropdown-toggle" data=
-toggle=3D"dropdown">Download as<span class=3D"sr-only">Dropdown</span></a>
                            <ul id=3D"download_menu" class=3D"dropdown-menu=
">
                               =20
                                <li id=3D"download_asciidoc">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>AsciiDoc (.asciidoc)</a>
                                </li>
                               =20
                                <li id=3D"download_html">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>HTML (.html)</a>
                                </li>
                               =20
                                <li id=3D"download_latex">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>LaTeX (.tex)</a>
                                </li>
                               =20
                                <li id=3D"download_markdown">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Markdown (.md)</a>
                                </li>
                               =20
                                <li id=3D"download_notebook">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Notebook (.ipynb)</a>
                                </li>
                               =20
                                <li id=3D"download_pdf">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>PDF via LaTeX (.pdf)</a>
                                </li>
                               =20
                                <li id=3D"download_rst">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>reST (.rst)</a>
                                </li>
                               =20
                                <li id=3D"download_script">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Python (.py)</a>
                                </li>
                               =20
                                <li id=3D"download_slides">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Reveal.js slides (.slides.html)</a>
                                </li>
                               =20
                                <li id=3D"download_webpdf">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>PDF via HTML (.html)</a>
                                </li>
                               =20
                            </ul>
                        </li>
                        <li class=3D"dropdown-submenu hidden" role=3D"none"=
><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20curr=
ency-crosses%20from%20investing.com%20#" role=3D"menuitem">Deploy as</a>
                            <ul id=3D"deploy_menu" class=3D"dropdown-menu">=
</ul>
                        </li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"trust_notebook" role=3D"none" title=3D"Tr=
ust the output of this notebook" class=3D"disabled">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Trusted Notebook</a></li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"close_and_halt" role=3D"none" title=3D"Sh=
utdown this notebook's kernel, and close this window">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Close and Halt</a></li>
                    </ul>
                </li>

                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" class=3D"dropdown-toggle" id=3D"editlink" data-toggle=3D"dropdown" aria=
-haspopup=3D"true" aria-controls=3D"edit_menu" aria-expanded=3D"false">Edit=
</a>
                    <ul id=3D"edit_menu" class=3D"dropdown-menu" role=3D"me=
nu" aria-labelledby=3D"editlink">
                        <li id=3D"cut_cell" role=3D"none"><a href=3D"http:/=
/localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20fro=
m%20investing.com%20#" role=3D"menuitem" class=3D"menu-shortcut-container">=
<span class=3D"action">Cut Cells</span><span class=3D"kb"><kbd>X</kbd></spa=
n></a></li>
                        <li id=3D"copy_cell" role=3D"none"><a href=3D"http:=
//localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20fr=
om%20investing.com%20#" role=3D"menuitem" class=3D"menu-shortcut-container"=
><span class=3D"action">Copy Cells</span><span class=3D"kb"><kbd>C</kbd></s=
pan></a></li>
                        <li id=3D"paste_cell_above" class=3D"" role=3D"none=
"><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20cur=
rency-crosses%20from%20investing.com%20#" role=3D"menuitem" aria-disabled=
=3D"false" class=3D"menu-shortcut-container"><span class=3D"action">Paste C=
ells Above</span><span class=3D"kb"><kbd>Shift-V</kbd></span></a></li>
                        <li id=3D"paste_cell_below" class=3D"" role=3D"none=
"><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20cur=
rency-crosses%20from%20investing.com%20#" role=3D"menuitem" aria-disabled=
=3D"false" class=3D"menu-shortcut-container"><span class=3D"action">Paste C=
ells Below</span><span class=3D"kb"><kbd>V</kbd></span></a></li>
                        <li id=3D"paste_cell_replace" class=3D"" role=3D"no=
ne"><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20c=
urrency-crosses%20from%20investing.com%20#" role=3D"menuitem" aria-disabled=
=3D"false">Paste Cells &amp; Replace</a></li>
                        <li id=3D"delete_cell" role=3D"none"><a href=3D"htt=
p://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20=
from%20investing.com%20#" role=3D"menuitem" class=3D"menu-shortcut-containe=
r"><span class=3D"action">Delete Cells</span><span class=3D"kb"><kbd>D</kbd=
>,<kbd>D</kbd></span></a></li>
                        <li id=3D"undelete_cell" class=3D"" role=3D"none"><=
a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20curren=
cy-crosses%20from%20investing.com%20#" role=3D"menuitem" aria-disabled=3D"f=
alse" class=3D"menu-shortcut-container"><span class=3D"action">Undo Delete =
Cells</span><span class=3D"kb"><kbd>Z</kbd></span></a></li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"split_cell" role=3D"none"><a href=3D"http=
://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20f=
rom%20investing.com%20#" role=3D"menuitem" class=3D"menu-shortcut-container=
"><span class=3D"action">Split Cell</span><span class=3D"kb"><kbd>Ctrl-Shif=
t-Minus</kbd></span></a></li>
                        <li id=3D"merge_cell_above" role=3D"none"><a href=
=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-cro=
sses%20from%20investing.com%20#" role=3D"menuitem">Merge Cell Above</a></li=
>
                        <li id=3D"merge_cell_below" role=3D"none"><a href=
=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-cro=
sses%20from%20investing.com%20#" role=3D"menuitem">Merge Cell Below</a></li=
>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"move_cell_up" role=3D"none"><a href=3D"ht=
tp://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%2=
0from%20investing.com%20#" role=3D"menuitem">Move Cell Up</a></li>
                        <li id=3D"move_cell_down" role=3D"none"><a href=3D"=
http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses=
%20from%20investing.com%20#" role=3D"menuitem">Move Cell Down</a></li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"edit_nb_metadata" role=3D"none"><a href=
=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-cro=
sses%20from%20investing.com%20#" role=3D"menuitem">Edit Notebook Metadata</=
a></li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"find_and_replace" role=3D"none"><a href=
=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-cro=
sses%20from%20investing.com%20#" role=3D"menuitem"> Find and Replace </a></=
li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"cut_cell_attachments" role=3D"none"><a hr=
ef=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-c=
rosses%20from%20investing.com%20#" role=3D"menuitem">Cut Cell Attachments</=
a></li>
                        <li id=3D"copy_cell_attachments" role=3D"none"><a h=
ref=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-=
crosses%20from%20investing.com%20#" role=3D"menuitem">Copy Cell Attachments=
</a></li>
                        <li id=3D"paste_cell_attachments" class=3D"disabled=
" role=3D"none"><a href=3D"http://localhost:8890/notebooks/Code%20for%20for=
ecasting%20currency-crosses%20from%20investing.com%20#" role=3D"menuitem" a=
ria-disabled=3D"true">Paste Cell Attachments</a></li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"insert_image" class=3D"disabled" role=3D"=
none"><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%2=
0currency-crosses%20from%20investing.com%20#" role=3D"menuitem" aria-disabl=
ed=3D"true">  Insert Image </a></li>
                    </ul>
                </li>
                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" class=3D"dropdown-toggle" id=3D"viewlink" data-toggle=3D"dropdown" aria=
-haspopup=3D"true" aria-controls=3D"view_menu" aria-expanded=3D"false">View=
</a>
                    <ul id=3D"view_menu" class=3D"dropdown-menu" role=3D"me=
nu" aria-labelledby=3D"viewlink">
                        <li id=3D"toggle_header" role=3D"none" title=3D"Sho=
w/Hide the logo and notebook title (above menu bar)">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Toggle Header</a>
                        </li>
                        <li id=3D"toggle_toolbar" role=3D"none" title=3D"Sh=
ow/Hide the action icons (below menu bar)">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Toggle Toolbar</a>
                        </li>
                        <li id=3D"toggle_line_numbers" role=3D"none" title=
=3D"Show/Hide line numbers in cells">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" class=3D"menu-shortcut-container"><span class=3D"action">Toggle =
Line Numbers</span><span class=3D"kb"><kbd>Shift-L</kbd></span></a>
                        </li>
                        <li id=3D"menu-cell-toolbar" class=3D"menu_focus_hi=
ghlight dropdown-submenu" role=3D"none">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" class=3D"dropdown=
-toggle" data-toggle=3D"dropdown">Cell Toolbar</a>
                            <ul class=3D"dropdown-menu" id=3D"menu-cell-too=
lbar-submenu"><li data-name=3D"None"><a href=3D"http://localhost:8890/noteb=
ooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#=
">None</a></li><li data-name=3D"Edit%20Metadata"><a href=3D"http://localhos=
t:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20from%20inves=
ting.com%20#">Edit Metadata</a></li><li data-name=3D"Raw%20Cell%20Format"><=
a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20curren=
cy-crosses%20from%20investing.com%20#">Raw Cell Format</a></li><li data-nam=
e=3D"Slideshow"><a href=3D"http://localhost:8890/notebooks/Code%20for%20for=
ecasting%20currency-crosses%20from%20investing.com%20#">Slideshow</a></li><=
li data-name=3D"Attachments"><a href=3D"http://localhost:8890/notebooks/Cod=
e%20for%20forecasting%20currency-crosses%20from%20investing.com%20#">Attach=
ments</a></li><li data-name=3D"Tags"><a href=3D"http://localhost:8890/noteb=
ooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#=
">Tags</a></li></ul>
                        </li>
                    </ul>
                </li>
                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" class=3D"dropdown-toggle" id=3D"insertlink" data-toggle=3D"dropdown" ar=
ia-haspopup=3D"true" aria-controls=3D"insert_menu" aria-expanded=3D"false">=
Insert</a>
                    <ul id=3D"insert_menu" class=3D"dropdown-menu" role=3D"=
menu" aria-labelledby=3D"insertlink">
                        <li id=3D"insert_cell_above" role=3D"none" title=3D=
"Insert an empty Code cell above the currently active cell">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" class=3D"menu-shortcut-container"><span class=3D"action">Insert =
Cell Above</span><span class=3D"kb"><kbd>A</kbd></span></a></li>
                        <li id=3D"insert_cell_below" role=3D"none" title=3D=
"Insert an empty Code cell below the currently active cell">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" class=3D"menu-shortcut-container"><span class=3D"action">Insert =
Cell Below</span><span class=3D"kb"><kbd>B</kbd></span></a></li>
                    </ul>
                </li>
                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" class=3D"dropdown-toggle" id=3D"celllink" data-toggle=3D"dropdown" aria=
-haspopup=3D"true" aria-controls=3D"cell_menu" aria-expanded=3D"false">Cell=
</a>
                    <ul id=3D"cell_menu" class=3D"dropdown-menu" role=3D"me=
nu" aria-labelledby=3D"celllink">
                        <li id=3D"run_cell" role=3D"none" title=3D"Run this=
 cell, and move cursor to the next one">
                            <a role=3D"menuitem" href=3D"http://localhost:8=
890/notebooks/Code%20for%20forecasting%20currency-crosses%20from%20investin=
g.com%20#" class=3D"menu-shortcut-container"><span class=3D"action">Run Cel=
ls</span><span class=3D"kb"><kbd>Ctrl-Enter</kbd></span></a></li>
                        <li id=3D"run_cell_select_below" role=3D"none" titl=
e=3D"Run this cell, select below">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" class=3D"menu-shortcut-container"><span class=3D"action">Run Cel=
ls and Select Below</span><span class=3D"kb"><kbd>Shift-Enter</kbd></span><=
/a></li>
                        <li id=3D"run_cell_insert_below" role=3D"none" titl=
e=3D"Run this cell, insert below">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" class=3D"menu-shortcut-container"><span class=3D"action">Run Cel=
ls and Insert Below</span><span class=3D"kb"><kbd>Alt-Enter</kbd></span></a=
></li>
                        <li id=3D"run_all_cells" role=3D"none" title=3D"Run=
 all cells in the notebook">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Run All</a></li>
                        <li id=3D"run_all_cells_above" role=3D"none" title=
=3D"Run all cells above (but not including) this cell">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Run All Above</a></li>
                        <li id=3D"run_all_cells_below" role=3D"none" title=
=3D"Run this cell and all cells below it">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem">Run All Below</a></li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"change_cell_type" class=3D"menu_focus_hig=
hlight dropdown-submenu" role=3D"none" title=3D"All cells in the notebook h=
ave a cell type. By default, new cells are created as 'Code' cells">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" class=3D"dropdown=
-toggle" data-toggle=3D"dropdown">Cell Type</a>
                            <ul class=3D"dropdown-menu" role=3D"menu">
                              <li id=3D"to_code" role=3D"none" title=3D"Con=
tents will be sent to the kernel for execution, and output will display in =
the footer of cell">
                                  <a href=3D"http://localhost:8890/notebook=
s/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" c=
lass=3D"menu-shortcut-container"><span class=3D"action">Code</span><span cl=
ass=3D"kb"><kbd>Y</kbd></span></a></li>
                              <li id=3D"to_markdown" title=3D"Contents will=
 be rendered as HTML and serve as explanatory text">
                                  <a href=3D"http://localhost:8890/notebook=
s/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" c=
lass=3D"menu-shortcut-container"><span class=3D"action">Markdown</span><spa=
n class=3D"kb"><kbd>M</kbd></span></a></li>
                              <li id=3D"to_raw" title=3D"Contents will pass=
 through nbconvert unmodified">
                                  <a href=3D"http://localhost:8890/notebook=
s/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" c=
lass=3D"menu-shortcut-container"><span class=3D"action">Raw NBConvert</span=
><span class=3D"kb"><kbd>R</kbd></span></a></li>
                            </ul>
                        </li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"current_outputs" class=3D"menu_focus_high=
light dropdown-submenu" role=3D"none"><a href=3D"http://localhost:8890/note=
books/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20=
#" role=3D"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" class=
=3D"dropdown-toggle" data-toggle=3D"dropdown">Current Outputs</a>
                            <ul class=3D"dropdown-menu" role=3D"menu">
                                <li id=3D"toggle_current_output" role=3D"no=
ne" title=3D"Hide/Show the output of the current cell">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
 class=3D"menu-shortcut-container"><span class=3D"action">Toggle</span><spa=
n class=3D"kb"><kbd>O</kbd></span></a>
                                </li>
                                <li id=3D"toggle_current_output_scroll" tit=
le=3D"Scroll the output of the current cell">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
 class=3D"menu-shortcut-container"><span class=3D"action">Toggle Scrolling<=
/span><span class=3D"kb"><kbd>Shift-O</kbd></span></a>
                                </li>
                                <li id=3D"clear_current_output" title=3D"Cl=
ear the output of the current cell">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Clear</a>
                                </li>
                            </ul>
                        </li>
                        <li id=3D"all_outputs" class=3D"menu_focus_highligh=
t dropdown-submenu" role=3D"none"><a href=3D"http://localhost:8890/notebook=
s/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" r=
ole=3D"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" class=3D"dr=
opdown-toggle" data-toggle=3D"dropdown">All Output</a>
                            <ul class=3D"dropdown-menu" role=3D"menu">
                                <li id=3D"toggle_all_output" role=3D"none" =
title=3D"Hide/Show the output of all cells">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Toggle</a>
                                </li>
                                <li id=3D"toggle_all_output_scroll" title=
=3D"Scroll the output of all cells">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Toggle Scrolling</a>
                                </li>
                                <li id=3D"clear_all_output" title=3D"Clear =
the output of all cells">
                                    <a href=3D"http://localhost:8890/notebo=
oks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#"=
>Clear</a>
                                </li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" class=3D"dropdown-toggle" data-toggle=3D"dropdown" id=3D"kernellink" ar=
ia-expanded=3D"false">Kernel</a>
                    <ul id=3D"kernel_menu" class=3D"dropdown-menu" aria-lab=
elledby=3D"kernellink">
                        <li id=3D"int_kernel" title=3D"Send Keyboard Interr=
upt (CTRL-C) to the Kernel">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" class=
=3D"menu-shortcut-container"><span class=3D"action">Interrupt</span><span c=
lass=3D"kb"><kbd>I</kbd>,<kbd>I</kbd></span></a>
                        </li>
                        <li id=3D"restart_kernel" title=3D"Restart the Kern=
el">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" class=
=3D"menu-shortcut-container"><span class=3D"action">Restart</span><span cla=
ss=3D"kb"><kbd>0</kbd>,<kbd>0</kbd></span></a>
                        </li>
                        <li id=3D"restart_clear_output" title=3D"Restart th=
e Kernel and clear all output">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#">Restart=
 &amp; Clear Output</a>
                        </li>
                        <li id=3D"restart_run_all" title=3D"Restart the Ker=
nel and re-run the notebook">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#">Restart=
 &amp; Run All</a>
                        </li>
                        <li id=3D"reconnect_kernel" title=3D"Reconnect to t=
he Kernel">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#">Reconne=
ct</a>
                        </li>
                        <li id=3D"shutdown_kernel" title=3D"Shutdown the Ke=
rnel">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#">Shutdow=
n</a>
                        </li>
                        <li class=3D"divider" role=3D"none"></li>
                        <li id=3D"menu-change-kernel" class=3D"menu_focus_h=
ighlight dropdown-submenu" role=3D"menuitem">
                            <a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" role=3D=
"menuitem" aria-haspopup=3D"true" aria-expanded=3D"false" class=3D"dropdown=
-toggle" data-toggle=3D"dropdown">Change kernel</a>
                            <ul class=3D"dropdown-menu" id=3D"menu-change-k=
ernel-submenu"><li id=3D"kernel-submenu-python3"><a href=3D"http://localhos=
t:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20from%20inves=
ting.com%20#">Python 3 (ipykernel)</a></li></ul>
                        </li>
                    </ul>
                </li>
                <li class=3D"dropdown"><a href=3D"http://localhost:8890/not=
ebooks/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%2=
0#" data-toggle=3D"dropdown" class=3D"dropdown-toggle" aria-expanded=3D"fal=
se">Widgets</a><ul id=3D"widget-submenu" class=3D"dropdown-menu"><li title=
=3D"Save the notebook with the widget state information for static renderin=
g"><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20cu=
rrency-crosses%20from%20investing.com%20#">Save Notebook Widget State</a></=
li><li title=3D"Clear the widget state information from the notebook"><a hr=
ef=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-c=
rosses%20from%20investing.com%20#">Clear Notebook Widget State</a></li><ul =
class=3D"divider"></ul><li title=3D"Download the widget state as a JSON fil=
e"><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20cu=
rrency-crosses%20from%20investing.com%20#">Download Widget State</a></li><l=
i title=3D"Embed interactive widgets"><a href=3D"http://localhost:8890/note=
books/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20=
#">Embed Widgets</a></li></ul></li><li class=3D"dropdown"><a href=3D"http:/=
/localhost:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20fro=
m%20investing.com%20#" class=3D"dropdown-toggle" data-toggle=3D"dropdown" a=
ria-expanded=3D"false">Help</a>
                    <ul id=3D"help_menu" class=3D"dropdown-menu">
                       =20
                        <li id=3D"notebook_tour" title=3D"A quick tour of t=
he notebook user interface"><a href=3D"http://localhost:8890/notebooks/Code=
%20for%20forecasting%20currency-crosses%20from%20investing.com%20#">User In=
terface Tour</a></li>
                        <li id=3D"keyboard_shortcuts" title=3D"Opens a tool=
tip with all keyboard shortcuts"><a href=3D"http://localhost:8890/notebooks=
/Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" cl=
ass=3D"menu-shortcut-container"><span class=3D"action">Keyboard Shortcuts</=
span><span class=3D"kb"><kbd>H</kbd></span></a></li>
                        <li id=3D"edit_keyboard_shortcuts" title=3D"Opens a=
 dialog allowing you to edit Keyboard shortcuts"><a href=3D"http://localhos=
t:8890/notebooks/Code%20for%20forecasting%20currency-crosses%20from%20inves=
ting.com%20#">Edit Keyboard Shortcuts</a></li>
                        <li class=3D"divider"></li>
                       =20

					=09
                       =20
                           =20
                                <li><a rel=3D"noreferrer" href=3D"http://nb=
viewer.jupyter.org/github/ipython/ipython/blob/3.x/examples/Notebook/Index.=
ipynb" target=3D"_blank" title=3D"Opens in a new window">
                               =20
                                    <i class=3D"fa fa-external-link menu-ic=
on pull-right"></i>
                               =20

                                Notebook Help
                                </a></li>
                           =20
                                <li><a rel=3D"noreferrer" href=3D"https://h=
elp.github.com/articles/markdown-basics/" target=3D"_blank" title=3D"Opens =
in a new window">
                               =20
                                    <i class=3D"fa fa-external-link menu-ic=
on pull-right"></i>
                               =20

                                Markdown
                                </a></li>
                           =20
                           =20
                       =20
                        <li id=3D"kernel-help-links" class=3D"divider"></li=
><li><a target=3D"_blank" title=3D"Opens in a new window" href=3D"https://d=
ocs.python.org/3.11?v=3D20240226232902"><i class=3D"fa fa-external-link men=
u-icon pull-right"></i><span>Python Reference</span></a></li><li><a target=
=3D"_blank" title=3D"Opens in a new window" href=3D"https://ipython.org/doc=
umentation.html?v=3D20240226232902"><i class=3D"fa fa-external-link menu-ic=
on pull-right"></i><span>IPython Reference</span></a></li><li><a target=3D"=
_blank" title=3D"Opens in a new window" href=3D"https://docs.scipy.org/doc/=
numpy/reference/?v=3D20240226232902"><i class=3D"fa fa-external-link menu-i=
con pull-right"></i><span>NumPy Reference</span></a></li><li><a target=3D"_=
blank" title=3D"Opens in a new window" href=3D"https://docs.scipy.org/doc/s=
cipy/reference/?v=3D20240226232902"><i class=3D"fa fa-external-link menu-ic=
on pull-right"></i><span>SciPy Reference</span></a></li><li><a target=3D"_b=
lank" title=3D"Opens in a new window" href=3D"https://matplotlib.org/conten=
ts.html?v=3D20240226232902"><i class=3D"fa fa-external-link menu-icon pull-=
right"></i><span>Matplotlib Reference</span></a></li><li><a target=3D"_blan=
k" title=3D"Opens in a new window" href=3D"http://docs.sympy.org/latest/ind=
ex.html?v=3D20240226232902"><i class=3D"fa fa-external-link menu-icon pull-=
right"></i><span>SymPy Reference</span></a></li><li><a target=3D"_blank" ti=
tle=3D"Opens in a new window" href=3D"https://pandas.pydata.org/pandas-docs=
/stable/?v=3D20240226232902"><i class=3D"fa fa-external-link menu-icon pull=
-right"></i><span>pandas Reference</span></a></li><li class=3D"divider"></l=
i>
                        <li title=3D"About Jupyter Notebook"><a id=3D"noteb=
ook_about" href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting=
%20currency-crosses%20from%20investing.com%20#">About</a></li>
                       =20
                    </ul>
                </li>
              </ul>
            </div>
        </div>
    </div>
</div>

<div id=3D"maintoolbar" class=3D"navbar">
  <div class=3D"toolbar-inner navbar-inner navbar-nobg">
    <div id=3D"maintoolbar-container" class=3D"container toolbar"><div clas=
s=3D"btn-group" id=3D"save-notbook"><button class=3D"btn btn-default" title=
=3D"Save and Checkpoint" data-jupyter-action=3D"jupyter-notebook:save-noteb=
ook"><i class=3D"fa-save fa"></i></button></div><div class=3D"btn-group" id=
=3D"insert_above_below"><button class=3D"btn btn-default" title=3D"insert c=
ell below" data-jupyter-action=3D"jupyter-notebook:insert-cell-below"><i cl=
ass=3D"fa-plus fa"></i></button></div><div class=3D"btn-group" id=3D"cut_co=
py_paste"><button class=3D"btn btn-default" title=3D"cut selected cells" da=
ta-jupyter-action=3D"jupyter-notebook:cut-cell"><i class=3D"fa-cut fa"></i>=
</button><button class=3D"btn btn-default" title=3D"copy selected cells" da=
ta-jupyter-action=3D"jupyter-notebook:copy-cell"><i class=3D"fa-copy fa"></=
i></button><button class=3D"btn btn-default" title=3D"paste cells below" da=
ta-jupyter-action=3D"jupyter-notebook:paste-cell-below"><i class=3D"fa-past=
e fa"></i></button></div><div class=3D"btn-group" id=3D"move_up_down"><butt=
on class=3D"btn btn-default" title=3D"move selected cells up" data-jupyter-=
action=3D"jupyter-notebook:move-cell-up"><i class=3D"fa-arrow-up fa"></i></=
button><button class=3D"btn btn-default" title=3D"move selected cells down"=
 data-jupyter-action=3D"jupyter-notebook:move-cell-down"><i class=3D"fa-arr=
ow-down fa"></i></button></div><div class=3D"btn-group" id=3D"run_int"><but=
ton class=3D"btn btn-default" aria-label=3D"Run" title=3D"run cell, select =
below" data-jupyter-action=3D"jupyter-notebook:run-cell-and-select-next"><i=
 class=3D"fa-play fa"></i><span class=3D"toolbar-btn-label">Run</span></but=
ton><button class=3D"btn btn-default" title=3D"interrupt the kernel" data-j=
upyter-action=3D"jupyter-notebook:interrupt-kernel"><i class=3D"fa-stop fa"=
></i></button><button class=3D"btn btn-default" title=3D"restart the kernel=
 (with dialog)" data-jupyter-action=3D"jupyter-notebook:confirm-restart-ker=
nel"><i class=3D"fa-repeat fa"></i></button><button class=3D"btn btn-defaul=
t" title=3D"restart the kernel, then re-run the whole notebook (with dialog=
)" data-jupyter-action=3D"jupyter-notebook:confirm-restart-kernel-and-run-a=
ll-cells"><i class=3D"fa-forward fa"></i></button></div><select id=3D"cell_=
type" aria-label=3D"combobox, select cell type" role=3D"combobox" class=3D"=
form-control select-xs"><option value=3D"code">Code</option><option value=
=3D"markdown">Markdown</option><option value=3D"raw">Raw NBConvert</option>=
<option value=3D"heading">Heading</option><option value=3D"multiselect" dis=
abled=3D"disabled" style=3D"display: none;">-</option></select><div class=
=3D"btn-group" id=3D"cmd_palette"><button class=3D"btn btn-default" title=
=3D"open the command palette" data-jupyter-action=3D"jupyter-notebook:show-=
command-palette"><i class=3D"fa-keyboard-o fa"></i></button></div></div>
  </div>
</div>
</div>

<div class=3D"lower-header-bar"></div>

</div>

<div id=3D"site" style=3D"display: block; height: 611.463px;">


<div id=3D"ipython-main-app">
    <div id=3D"notebook_panel">
        <div id=3D"notebook" tabindex=3D"-1"><div class=3D"container" id=3D=
"notebook-container"><div class=3D"cell code_cell rendered unselected" tabi=
ndex=3D"2"><div class=3D"input"><div class=3D"prompt_container"><div class=
=3D"prompt input_prompt"><bdi>In</bdi>&nbsp;[9]:</div><div class=3D"run_thi=
s_cell" title=3D"Run this cell"><i class=3D"fa-step-forward fa"></i></div><=
/div><div class=3D"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"ce=
lltoolbar"></div></div><div class=3D"input_area" aria-label=3D"Edit code he=
re"><div class=3D"CodeMirror cm-s-ipython"><div style=3D"overflow: hidden; =
position: relative; width: 3px; height: 0px; top: 39.6px; left: 245.856px;"=
><textarea autocorrect=3D"off" autocapitalize=3D"off" spellcheck=3D"false" =
tabindex=3D"0" style=3D"position: absolute; bottom: -1em; padding: 0px; wid=
th: 1000px; height: 1em; outline: none;"></textarea></div><div class=3D"Cod=
eMirror-vscrollbar" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"m=
in-width: 1px; height: 0px;"></div></div><div class=3D"CodeMirror-hscrollba=
r" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"height: 100%; min-=
height: 1px; width: 0px;"></div></div><div class=3D"CodeMirror-scrollbar-fi=
ller" cm-not-content=3D"true"></div><div class=3D"CodeMirror-gutter-filler"=
 cm-not-content=3D"true"></div><div class=3D"CodeMirror-scroll" tabindex=3D=
"-1"><div class=3D"CodeMirror-sizer" style=3D"margin-left: 34px; min-width:=
 361.1px; margin-bottom: -17px; border-right-width: 33px; min-height: 198px=
; padding-right: 0px; padding-bottom: 0px;"><div style=3D"position: relativ=
e; top: 0px;"><div class=3D"CodeMirror-lines" role=3D"presentation"><div ro=
le=3D"presentation" style=3D"position: relative; outline: none;"><div class=
=3D"CodeMirror-measure"><div class=3D"CodeMirror-linenumber CodeMirror-gutt=
er-elt"><div>11</div></div></div><div class=3D"CodeMirror-measure"></div><d=
iv style=3D"position: relative; z-index: 1;"></div><div class=3D"CodeMirror=
-cursors" style=3D""><div class=3D"CodeMirror-cursor" style=3D"left: 211.85=
6px; top: 34px; height: 17px;">&nbsp;</div></div><div class=3D"CodeMirror-c=
ode" role=3D"presentation" style=3D""><div style=3D"position: relative;"><d=
iv class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D=
"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21=
px;">1</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><s=
pan role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm=
-keyword">import</span> <span class=3D"cm-variable">urllib3</span></span></=
pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutte=
r-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeM=
irror-gutter-elt" style=3D"left: 0px; width: 21px;">2</div></div><pre class=
=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" st=
yle=3D"padding-right: 0.1px;"><span class=3D"cm-keyword">import</span> <spa=
n class=3D"cm-variable">gc</span></span></pre></div><div style=3D"position:=
 relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"=
><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: =
0px; width: 21px;">3</div></div><pre class=3D" CodeMirror-line " role=3D"pr=
esentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><sp=
an class=3D"cm-keyword">from</span> <span class=3D"cm-variable">time</span>=
 <span class=3D"cm-keyword">import</span> <span class=3D"cm-variable">time<=
/span>,<span class=3D"cm-variable">sleep</span></span></pre></div><div styl=
e=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D=
"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" s=
tyle=3D"left: 0px; width: 21px;">4</div></div><pre class=3D" CodeMirror-lin=
e " role=3D"presentation"><span role=3D"presentation" style=3D"padding-righ=
t: 0.1px;"><span class=3D"cm-keyword">import</span> <span class=3D"cm-varia=
ble">warnings</span></span></pre></div><div style=3D"position: relative;"><=
div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">5</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"=
><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D=
"cm-variable">warnings</span>.<span class=3D"cm-property">filterwarnings</s=
pan>(<span class=3D"cm-string">"ignore"</span>)</span></pre></div><div styl=
e=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D=
"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" s=
tyle=3D"left: 0px; width: 21px;">6</div></div><pre class=3D" CodeMirror-lin=
e " role=3D"presentation"><span role=3D"presentation" style=3D"padding-righ=
t: 0.1px;"><span class=3D"cm-keyword">import</span> <span class=3D"cm-varia=
ble">pandas</span> <span class=3D"cm-keyword">as</span> <span class=3D"cm-v=
ariable">pd</span></span></pre></div><div style=3D"position: relative;"><di=
v class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"=
CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21p=
x;">7</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><sp=
an role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-=
variable">urllib3</span>.<span class=3D"cm-property">disable_warnings</span=
>()</span></pre></div><div style=3D"position: relative;"><div class=3D"Code=
Mirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-line=
number CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">8</div></di=
v><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"pres=
entation" style=3D"padding-right: 0.1px;"><span class=3D"cm-keyword">import=
</span> <span class=3D"cm-variable">matplotlib</span>.<span class=3D"cm-pro=
perty">pyplot</span> <span class=3D"cm-keyword">as</span> <span class=3D"cm=
-variable">plt</span></span></pre></div><div style=3D"position: relative;">=
<div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">9</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"=
><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D=
"cm-keyword">import</span> <span class=3D"cm-variable">numpy</span> <span c=
lass=3D"cm-keyword">as</span> <span class=3D"cm-variable">np</span></span><=
/pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutt=
er-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Code=
Mirror-gutter-elt" style=3D"left: 0px; width: 21px;">10</div></div><pre cla=
ss=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" =
style=3D"padding-right: 0.1px;"><span class=3D"cm-keyword">from</span> <spa=
n class=3D"cm-variable">statsmodels</span>.<span class=3D"cm-property">tsa<=
/span>.<span class=3D"cm-property">arima</span>.<span class=3D"cm-property"=
>model</span> <span class=3D"cm-keyword">import</span> <span class=3D"cm-va=
riable">ARIMA</span></span></pre></div><div style=3D"position: relative;"><=
div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">11</div></div><pre class=3D" CodeMirror-line " role=3D"presentation=
"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-keyword">from</span> <span class=3D"cm-variable">sklearn</span>.<spa=
n class=3D"cm-property">metrics</span> <span class=3D"cm-keyword">import</s=
pan> <span class=3D"cm-variable">mean_squared_error</span></span></pre></di=
v></div></div></div></div></div><div style=3D"position: absolute; height: 3=
3px; width: 1px; border-bottom: 0px solid transparent; top: 198px;"></div><=
div class=3D"CodeMirror-gutters" style=3D"height: 231px; left: 0px;"><div c=
lass=3D"CodeMirror-gutter CodeMirror-linenumbers" style=3D"width: 33px;"></=
div></div></div></div></div></div></div><div class=3D"output_wrapper"><div =
class=3D"out_prompt_overlay prompt" title=3D"click to scroll output; double=
 click to hide"></div><div class=3D"output"></div><div class=3D"btn btn-def=
ault output_collapsed" title=3D"click to expand output" style=3D"display: n=
one;">. . .</div></div></div><div class=3D"cell code_cell rendered unselect=
ed" tabindex=3D"2"><div class=3D"input"><div class=3D"prompt_container"><di=
v class=3D"prompt input_prompt"><bdi>In</bdi>&nbsp;[10]:</div><div class=3D=
"run_this_cell" title=3D"Run this cell"><i class=3D"fa-step-forward fa"></i=
></div></div><div class=3D"inner_cell"><div class=3D"ctb_hideshow"><div cla=
ss=3D"celltoolbar"></div></div><div class=3D"input_area" aria-label=3D"Edit=
 code here"><div class=3D"CodeMirror cm-s-ipython"><div style=3D"overflow: =
hidden; position: relative; width: 3px; height: 0px; top: 1484.6px; left: 6=
8.7937px;"><textarea autocorrect=3D"off" autocapitalize=3D"off" spellcheck=
=3D"false" tabindex=3D"0" style=3D"position: absolute; bottom: -1em; paddin=
g: 0px; width: 1000px; height: 1em; outline: none;"></textarea></div><div c=
lass=3D"CodeMirror-vscrollbar" tabindex=3D"-1" cm-not-content=3D"true" styl=
e=3D"bottom: 0px;"><div style=3D"min-width: 1px; height: 0px;"></div></div>=
<div class=3D"CodeMirror-hscrollbar" tabindex=3D"-1" cm-not-content=3D"true=
" style=3D"right: 0px; left: 34px; display: block;"><div style=3D"height: 1=
00%; min-height: 1px; width: 930.788px;"></div></div><div class=3D"CodeMirr=
or-scrollbar-filler" cm-not-content=3D"true"></div><div class=3D"CodeMirror=
-gutter-filler" cm-not-content=3D"true"></div><div class=3D"CodeMirror-scro=
ll" tabindex=3D"-1"><div class=3D"CodeMirror-sizer" style=3D"margin-left: 3=
4px; min-width: 930.788px; margin-bottom: -17px; border-right-width: 33px; =
min-height: 1507px; padding-right: 0px; padding-bottom: 17px;"><div style=
=3D"position: relative; top: 0px;"><div class=3D"CodeMirror-lines" role=3D"=
presentation"><div role=3D"presentation" style=3D"position: relative; outli=
ne: none;"><div class=3D"CodeMirror-measure"><div class=3D"CodeMirror-linen=
umber CodeMirror-gutter-elt"><div>88</div></div></div><div class=3D"CodeMir=
ror-measure"></div><div style=3D"position: relative; z-index: 1;"></div><di=
v class=3D"CodeMirror-cursors" style=3D""><div class=3D"CodeMirror-cursor" =
style=3D"left: 34.7937px; top: 1479px; height: 17px;">&nbsp;</div></div><di=
v class=3D"CodeMirror-code" role=3D"presentation" style=3D""><div style=3D"=
position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left=
: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=
=3D"left: 0px; width: 21px;">1</div></div><pre class=3D" CodeMirror-line " =
role=3D"presentation"><span role=3D"presentation" style=3D"padding-right: 0=
.1px;"><span class=3D"cm-keyword">class</span> <span class=3D"cm-def">pred<=
/span>:</span></pre></div><div style=3D"position: relative;"><div class=3D"=
CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-=
linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">2</div>=
</div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"=
presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-keyword">def</=
span> <span class=3D"cm-def">__init__</span>(<span class=3D"cm-variable-2">=
self</span>):</span></pre></div><div style=3D"position: relative;"><div cla=
ss=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeM=
irror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">3=
</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span ro=
le=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" =
role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-keyword">retur=
n</span></span></pre></div><div style=3D"position: relative;"><div class=3D=
"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror=
-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">4</div=
></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D=
"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-keyword">def</=
span> <span class=3D"cm-def">getData</span>(<span class=3D"cm-variable-2">s=
elf</span>,<span class=3D"cm-variable">fi1</span>):</span></pre></div><div =
style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" styl=
e=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-el=
t" style=3D"left: 0px; width: 21px;">5</div></div><pre class=3D" CodeMirror=
-line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-=
right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"> =
   </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </=
span><span class=3D"cm-variable">htt</span><span class=3D"cm-operator">=3D<=
/span><span class=3D"cm-variable">urllib3</span>.<span class=3D"cm-property=
">PoolManager</span>()</span></pre></div><div style=3D"position: relative;"=
><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">6</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"=
><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D=
"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-t=
ab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variab=
le">ml</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-vari=
able">htt</span>.<span class=3D"cm-property">request</span>(<span class=3D"=
cm-string">'GET'</span>, <span class=3D"cm-variable">fi1</span>)</span></pr=
e></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutter-=
wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMir=
ror-gutter-elt" style=3D"left: 0px; width: 21px;">7</div></div><pre class=
=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" st=
yle=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-variable">ml</span><span class=3D"cm-=
operator">=3D</span><span class=3D"cm-variable">ml</span>.<span class=3D"cm=
-property">data</span></span></pre></div><div style=3D"position: relative;"=
><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">8</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"=
><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D=
"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-t=
ab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variab=
le">da</span><span class=3D"cm-operator">=3D</span><span class=3D"cm-builti=
n">str</span>(<span class=3D"cm-variable">ml</span>)</span></pre></div><div=
 style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" sty=
le=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-e=
lt" style=3D"left: 0px; width: 21px;">9</div></div><pre class=3D" CodeMirro=
r-line " role=3D"presentation"><span role=3D"presentation" style=3D"padding=
-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">=
    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    <=
/span><span class=3D"cm-keyword">return</span> <span class=3D"cm-variable">=
da</span></span></pre></div><div style=3D"position: relative;"><div class=
=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMir=
ror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">10<=
/div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span rol=
e=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" r=
ole=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-keyword">de=
f</span> <span class=3D"cm-def">reformat</span>(<span class=3D"cm-variable-=
2">self</span>,<span class=3D"cm-variable">da</span>):</span></pre></div><d=
iv style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" s=
tyle=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter=
-elt" style=3D"left: 0px; width: 21px;">11</div></div><pre class=3D" CodeMi=
rror-line " role=3D"presentation"><span role=3D"presentation" style=3D"padd=
ing-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"=
	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">  =
  </span><span class=3D"cm-variable">i</span><span class=3D"cm-operator">=
=3D</span><span class=3D"cm-number">0</span></span></pre></div><div style=
=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"=
left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" st=
yle=3D"left: 0px; width: 21px;">12</div></div><pre class=3D" CodeMirror-lin=
e " role=3D"presentation"><span role=3D"presentation" style=3D"padding-righ=
t: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    <=
/span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span=
><span class=3D"cm-variable">FD</span><span class=3D"cm-operator">=3D</span=
>[]</span></pre></div><div style=3D"position: relative;"><div class=3D"Code=
Mirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-line=
number CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">13</div></d=
iv><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"pre=
sentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-variable">lis</span><spa=
n class=3D"cm-operator">=3D</span>[]</span></pre></div><div style=3D"positi=
on: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34p=
x;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"lef=
t: 0px; width: 21px;">14</div></div><pre class=3D" CodeMirror-line " role=
=3D"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1px=
;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span c=
lass=3D"cm-keyword">while</span> <span class=3D"cm-variable">i</span><span =
class=3D"cm-operator">&lt;</span><span class=3D"cm-builtin">len</span>(<spa=
n class=3D"cm-variable">da</span>):</span></pre></div><div style=3D"positio=
n: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px=
;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left=
: 0px; width: 21px;">15</div></div><pre class=3D" CodeMirror-line " role=3D=
"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;">=
<span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span=
 class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span clas=
s=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"=
cm-variable">i</span><span class=3D"cm-operator">=3D</span><span class=3D"c=
m-variable">da</span>.<span class=3D"cm-property">index</span>(<span class=
=3D"cm-string">'&lt;time dateTime=3D'</span>,<span class=3D"cm-variable">i<=
/span><span class=3D"cm-operator">+</span><span class=3D"cm-number">1</span=
>,<span class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">da</spa=
n>))</span></pre></div><div style=3D"position: relative;"><div class=3D"Cod=
eMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-lin=
enumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">16</div></=
div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"pr=
esentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"=
presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"prese=
ntation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentati=
on" cm-text=3D"	">    </span><span class=3D"cm-keyword">if</span> <span cla=
ss=3D"cm-string">'&lt;time dateTime=3D'</span> <span class=3D"cm-keyword">i=
n</span> <span class=3D"cm-variable">da</span>[<span class=3D"cm-variable">=
i</span>:<span class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">=
da</span>)] <span class=3D"cm-keyword">and</span> <span class=3D"cm-variabl=
e">da</span>[<span class=3D"cm-variable">i</span>:<span class=3D"cm-variabl=
e">i</span><span class=3D"cm-operator">+</span><span class=3D"cm-number">15=
</span>]<span class=3D"cm-operator">=3D=3D</span><span class=3D"cm-string">=
'&lt;time dateTime=3D'</span> <span class=3D"cm-keyword">and</span> <span c=
lass=3D"cm-variable">da</span>[<span class=3D"cm-variable">i</span><span cl=
ass=3D"cm-operator">+</span><span class=3D"cm-number">26</span>:<span class=
=3D"cm-variable">i</span><span class=3D"cm-operator">+</span><span class=3D=
"cm-number">28</span>]<span class=3D"cm-operator">=3D=3D</span><span class=
=3D"cm-string">'"&gt;'</span>:</span></pre></div><div style=3D"position: re=
lative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><d=
iv class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px=
; width: 21px;">17</div></div><pre class=3D" CodeMirror-line " role=3D"pres=
entation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span=
 class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span clas=
s=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"=
cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-ta=
b" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variabl=
e">lis</span>.<span class=3D"cm-property">append</span>(<span class=3D"cm-v=
ariable">da</span>[<span class=3D"cm-variable">i</span><span class=3D"cm-op=
erator">+</span><span class=3D"cm-number">16</span>:<span class=3D"cm-varia=
ble">i</span><span class=3D"cm-operator">+</span><span class=3D"cm-number">=
26</span>])</span></pre></div><div style=3D"position: relative;"><div class=
=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMir=
ror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">18<=
/div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span rol=
e=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" r=
ole=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-keyword">if</span> <span=
 class=3D"cm-string">'text-positive-main" dir=3D"ltr"&gt;'</span> <span cla=
ss=3D"cm-keyword">in</span> <span class=3D"cm-variable">da</span>[<span cla=
ss=3D"cm-variable">i</span>:<span class=3D"cm-variable">i</span><span class=
=3D"cm-operator">+</span><span class=3D"cm-number">1305</span>]:</span></pr=
e></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutter-=
wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMir=
ror-gutter-elt" style=3D"left: 0px; width: 21px;">19</div></div><pre class=
=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" st=
yle=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D=
"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"> =
   </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </=
span><span class=3D"cm-variable">ix2</span><span class=3D"cm-operator">=3D<=
/span><span class=3D"cm-variable">da</span>.<span class=3D"cm-property">ind=
ex</span>(<span class=3D"cm-string">'text-positive-main" dir=3D"ltr"&gt;'</=
span>,<span class=3D"cm-variable">i</span>,<span class=3D"cm-variable">i</s=
pan><span class=3D"cm-operator">+</span><span class=3D"cm-number">1305</spa=
n>)</span></pre></div><div style=3D"position: relative;"><div class=3D"Code=
Mirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-line=
number CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">20</div></d=
iv><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"pre=
sentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-keyword">if</span> <span class=3D"=
cm-string">'text-negative-main" dir=3D"ltr"&gt;'</span> <span class=3D"cm-k=
eyword">in</span> <span class=3D"cm-variable">da</span>[<span class=3D"cm-v=
ariable">i</span>:<span class=3D"cm-variable">i</span><span class=3D"cm-ope=
rator">+</span><span class=3D"cm-number">1305</span>]:</span></pre></div><d=
iv style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" s=
tyle=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter=
-elt" style=3D"left: 0px; width: 21px;">21</div></div><pre class=3D" CodeMi=
rror-line " role=3D"presentation"><span role=3D"presentation" style=3D"padd=
ing-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"=
	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">  =
  </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </s=
pan><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><=
span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span =
class=3D"cm-variable">ix2</span><span class=3D"cm-operator">=3D</span><span=
 class=3D"cm-variable">da</span>.<span class=3D"cm-property">index</span>(<=
span class=3D"cm-string">'text-negative-main" dir=3D"ltr"&gt;'</span>,<span=
 class=3D"cm-variable">i</span>,<span class=3D"cm-variable">i</span><span c=
lass=3D"cm-operator">+</span><span class=3D"cm-number">1305</span>)</span><=
/pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutt=
er-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Code=
Mirror-gutter-elt" style=3D"left: 0px; width: 21px;">22</div></div><pre cla=
ss=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" =
style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation=
" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-=
text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=
=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	=
">    </span><span class=3D"cm-keyword">if</span> <span class=3D"cm-string"=
>'text-positive-main" dir=3D"ltr"&gt;'</span> <span class=3D"cm-keyword">in=
</span> <span class=3D"cm-variable">da</span>[<span class=3D"cm-variable">i=
</span>:<span class=3D"cm-variable">i</span><span class=3D"cm-operator">+</=
span><span class=3D"cm-number">1305</span>] <span class=3D"cm-keyword">or</=
span> <span class=3D"cm-string">'text-negative-main" dir=3D"ltr"&gt;'</span=
> <span class=3D"cm-keyword">in</span> <span class=3D"cm-variable">da</span=
>[<span class=3D"cm-variable">i</span>:<span class=3D"cm-variable">i</span>=
<span class=3D"cm-operator">+</span><span class=3D"cm-number">1305</span>]:=
</span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMir=
ror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenum=
ber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">23</div></div>=
<pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presen=
tation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"pres=
entation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentat=
ion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D=
"	">    </span><span class=3D"cm-variable">ix3</span><span class=3D"cm-oper=
ator">=3D</span><span class=3D"cm-variable">da</span>.<span class=3D"cm-pro=
perty">index</span>(<span class=3D"cm-string">'&lt;/td&gt;'</span>,<span cl=
ass=3D"cm-variable">ix2</span>,<span class=3D"cm-builtin">len</span>(<span =
class=3D"cm-variable">da</span>))</span></pre></div><div style=3D"position:=
 relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"=
><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: =
0px; width: 21px;">24</div></div><pre class=3D" CodeMirror-line " role=3D"p=
resentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><s=
pan class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span c=
lass=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab=
" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variable=
">lis</span>.<span class=3D"cm-property">append</span>(<span class=3D"cm-va=
riable">da</span>[<span class=3D"cm-variable">ix2</span><span class=3D"cm-o=
perator">+</span><span class=3D"cm-number">30</span>:<span class=3D"cm-vari=
able">ix3</span>])</span></pre></div><div style=3D"position: relative;"><di=
v class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"=
CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21p=
x;">25</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><s=
pan role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm=
-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab"=
 role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-keyword">for</span> <spa=
n class=3D"cm-variable">k</span> <span class=3D"cm-keyword">in</span> <span=
 class=3D"cm-builtin">range</span>(<span class=3D"cm-number">0</span>,<span=
 class=3D"cm-number">3</span>):</span></pre></div><div style=3D"position: r=
elative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><=
div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0p=
x; width: 21px;">26</div></div><pre class=3D" CodeMirror-line " role=3D"pre=
sentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><spa=
n class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span cla=
ss=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D=
"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-t=
ab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" r=
ole=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variable">j</s=
pan><span class=3D"cm-operator">=3D</span><span class=3D"cm-variable">ix3</=
span></span></pre></div><div style=3D"position: relative;"><div class=3D"Co=
deMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-li=
nenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">27</div><=
/div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"p=
resentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D=
"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"pres=
entation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentat=
ion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D=
"	">    </span><span class=3D"cm-variable">ix2</span><span class=3D"cm-oper=
ator">=3D</span><span class=3D"cm-variable">da</span>.<span class=3D"cm-pro=
perty">index</span>(<span class=3D"cm-string">'test=3D"relative-most-active=
-last"&gt;'</span>,<span class=3D"cm-variable">j</span>,<span class=3D"cm-b=
uiltin">len</span>(<span class=3D"cm-variable">da</span>))</span></pre></di=
v><div style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrappe=
r" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gu=
tter-elt" style=3D"left: 0px; width: 21px;">28</div></div><pre class=3D" Co=
deMirror-line " role=3D"presentation"><span role=3D"presentation" style=3D"=
padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=
=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	=
">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">   =
 </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </sp=
an><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span c=
lass=3D"cm-variable">ix3</span><span class=3D"cm-operator">=3D</span><span =
class=3D"cm-variable">da</span>.<span class=3D"cm-property">index</span>(<s=
pan class=3D"cm-string">'&lt;/td&gt;'</span>,<span class=3D"cm-variable">ix=
2</span>,<span class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">=
da</span>))</span></pre></div><div style=3D"position: relative;"><div class=
=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMir=
ror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">29<=
/div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span rol=
e=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" r=
ole=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-variable">lis</span>.<span class=
=3D"cm-property">append</span>(<span class=3D"cm-variable">da</span>[<span =
class=3D"cm-variable">ix2</span><span class=3D"cm-operator">+</span><span c=
lass=3D"cm-number">33</span>:<span class=3D"cm-variable">ix3</span>])</span=
></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gu=
tter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Co=
deMirror-gutter-elt" style=3D"left: 0px; width: 21px;">30</div></div><pre c=
lass=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation=
" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentati=
on" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" c=
m-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-tex=
t=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"=
	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">  =
  </span><span class=3D"cm-variable">FD</span>.<span class=3D"cm-property">=
append</span>(<span class=3D"cm-variable">lis</span>)</span></pre></div><di=
v style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" st=
yle=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-=
elt" style=3D"left: 0px; width: 21px;">31</div></div><pre class=3D" CodeMir=
ror-line " role=3D"presentation"><span role=3D"presentation" style=3D"paddi=
ng-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	=
">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">   =
 </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </sp=
an><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span c=
lass=3D"cm-variable">lis</span><span class=3D"cm-operator">=3D</span>[]</sp=
an></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-=
gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber =
CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">32</div></div><pre=
 class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentati=
on" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presenta=
tion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation"=
 cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-t=
ext=3D"	">    </span><span class=3D"cm-keyword">if</span> <span class=3D"cm=
-string">'&lt;time dateTime=3D'</span> <span class=3D"cm-keyword">not</span=
> <span class=3D"cm-keyword">in</span> <span class=3D"cm-variable">da</span=
>[<span class=3D"cm-variable">i</span><span class=3D"cm-operator">+</span><=
span class=3D"cm-number">1</span>:<span class=3D"cm-builtin">len</span>(<sp=
an class=3D"cm-variable">da</span>)]:</span></pre></div><div style=3D"posit=
ion: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34=
px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"le=
ft: 0px; width: 21px;">33</div></div><pre class=3D" CodeMirror-line " role=
=3D"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1px=
;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span c=
lass=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-keyword">break</span></span></pre></div><div style=3D"position: relative;=
"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div clas=
s=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width=
: 21px;">34</div></div><pre class=3D" CodeMirror-line " role=3D"presentatio=
n"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-var=
iable">FD</span>.<span class=3D"cm-property">reverse</span>()</span></pre><=
/div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wra=
pper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror=
-gutter-elt" style=3D"left: 0px; width: 21px;">35</div></div><pre class=3D"=
 CodeMirror-line " role=3D"presentation"><span role=3D"presentation" style=
=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-=
text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=
=3D"	">    </span><span class=3D"cm-variable">FD</span><span class=3D"cm-op=
erator">=3D</span>[<span class=3D"cm-variable">FD</span>[<span class=3D"cm-=
variable">i</span>][<span class=3D"cm-number">0</span>].<span class=3D"cm-p=
roperty">split</span>(<span class=3D"cm-string">'/'</span>)<span class=3D"c=
m-operator">+</span><span class=3D"cm-variable">FD</span>[<span class=3D"cm=
-variable">i</span>][<span class=3D"cm-number">1</span>:<span class=3D"cm-n=
umber">5</span>] <span class=3D"cm-keyword">for</span> <span class=3D"cm-va=
riable">i</span> <span class=3D"cm-keyword">in</span> <span class=3D"cm-bui=
ltin">range</span>(<span class=3D"cm-builtin">len</span>(<span class=3D"cm-=
variable">FD</span>))]</span></pre></div><div style=3D"position: relative;"=
><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">36</div></div><pre class=3D" CodeMirror-line " role=3D"presentation=
"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-var=
iable">Reformated_data</span> <span class=3D"cm-operator">=3D</span> {</spa=
n></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-g=
utter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber C=
odeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">37</div></div><pre =
class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentatio=
n" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentat=
ion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-string">"Month"</span>:[<span class=
=3D"cm-builtin">int</span>(<span class=3D"cm-variable">FD</span>[<span clas=
s=3D"cm-variable">i</span>][<span class=3D"cm-number">0</span>]) <span clas=
s=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span clas=
s=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span cl=
ass=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))],</sp=
an></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-=
gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber =
CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">38</div></div><pre=
 class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentati=
on" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presenta=
tion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation"=
 cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-t=
ext=3D"	">    </span><span class=3D"cm-string">"Day"</span>:[<span class=3D=
"cm-builtin">int</span>(<span class=3D"cm-variable">FD</span>[<span class=
=3D"cm-variable">i</span>][<span class=3D"cm-number">1</span>]) <span class=
=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span class=
=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span cla=
ss=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))],</spa=
n></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-g=
utter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber C=
odeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">39</div></div><pre =
class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentatio=
n" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentat=
ion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-string">"Year"</span>:[<span class=3D=
"cm-builtin">int</span>(<span class=3D"cm-variable">FD</span>[<span class=
=3D"cm-variable">i</span>][<span class=3D"cm-number">2</span>]) <span class=
=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span class=
=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span cla=
ss=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))],</spa=
n></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-g=
utter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber C=
odeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">40</div></div><pre =
class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentatio=
n" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentat=
ion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-string">"Price"</span>:[<span class=
=3D"cm-builtin">float</span>(<span class=3D"cm-variable">FD</span>[<span cl=
ass=3D"cm-variable">i</span>][<span class=3D"cm-number">3</span>]) <span cl=
ass=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span cl=
ass=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span =
class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))],</=
span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirro=
r-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumbe=
r CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">41</div></div><p=
re class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presenta=
tion" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-string">"Open"</span>:[<span class=
=3D"cm-builtin">float</span>(<span class=3D"cm-variable">FD</span>[<span cl=
ass=3D"cm-variable">i</span>][<span class=3D"cm-number">4</span>]) <span cl=
ass=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span cl=
ass=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span =
class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))],</=
span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirro=
r-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumbe=
r CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">42</div></div><p=
re class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presenta=
tion" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-string">"High"</span>:[<span class=
=3D"cm-builtin">float</span>(<span class=3D"cm-variable">FD</span>[<span cl=
ass=3D"cm-variable">i</span>][<span class=3D"cm-number">5</span>]) <span cl=
ass=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span cl=
ass=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span =
class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))],</=
span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirro=
r-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumbe=
r CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">43</div></div><p=
re class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presenta=
tion" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presen=
tation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-string">"Low"</span>:[<span class=
=3D"cm-builtin">float</span>(<span class=3D"cm-variable">FD</span>[<span cl=
ass=3D"cm-variable">i</span>][<span class=3D"cm-number">6</span>]) <span cl=
ass=3D"cm-keyword">for</span> <span class=3D"cm-variable">i</span> <span cl=
ass=3D"cm-keyword">in</span> <span class=3D"cm-builtin">range</span>(<span =
class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">FD</span>))]</s=
pan></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror=
-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber=
 CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">44</div></div><pr=
e class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentat=
ion" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"present=
ation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation=
" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-=
text=3D"	">    </span>}</span></pre></div><div style=3D"position: relative;=
"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div clas=
s=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width=
: 21px;">45</div></div><pre class=3D" CodeMirror-line " role=3D"presentatio=
n"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-var=
iable">PriceData</span> <span class=3D"cm-operator">=3D</span> <span class=
=3D"cm-variable">pd</span>.<span class=3D"cm-property">DataFrame</span>(<sp=
an class=3D"cm-variable">Reformated_data</span>)</span></pre></div><div sty=
le=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=
=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt=
" style=3D"left: 0px; width: 21px;">46</div></div><pre class=3D" CodeMirror=
-line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-=
right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"> =
   </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </=
span><span class=3D"cm-keyword">return</span> <span class=3D"cm-variable">P=
riceData</span></span></pre></div><div style=3D"position: relative;"><div c=
lass=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"Cod=
eMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;"=
>47</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span=
 role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-ta=
b" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-keyword=
">def</span> <span class=3D"cm-def">estim</span>(<span class=3D"cm-variable=
-2">self</span>,<span class=3D"cm-variable">PriceData</span>):</span></pre>=
</div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wr=
apper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirro=
r-gutter-elt" style=3D"left: 0px; width: 21px;">48</div></div><pre class=3D=
" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" style=
=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-=
text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=
=3D"	">    </span><span class=3D"cm-variable">model</span> <span class=3D"c=
m-operator">=3D</span> <span class=3D"cm-variable">ARIMA</span>(<span class=
=3D"cm-variable">PriceData</span>[<span class=3D"cm-string">'Low'</span>], =
<span class=3D"cm-variable">order</span><span class=3D"cm-operator">=3D</sp=
an>(<span class=3D"cm-number">1</span>, <span class=3D"cm-number">1</span>,=
 <span class=3D"cm-number">1</span>))</span></pre></div><div style=3D"posit=
ion: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34=
px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"le=
ft: 0px; width: 21px;">49</div></div><pre class=3D" CodeMirror-line " role=
=3D"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1px=
;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span c=
lass=3D"cm-variable">model_fit</span> <span class=3D"cm-operator">=3D</span=
> <span class=3D"cm-variable">model</span>.<span class=3D"cm-property">fit<=
/span>()</span></pre></div><div style=3D"position: relative;"><div class=3D=
"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror=
-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">50</di=
v></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=
=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" ro=
le=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D=
"presentation" cm-text=3D"	">    </span><span class=3D"cm-variable">forecas=
t</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-variable"=
>model_fit</span>.<span class=3D"cm-property">get_forecast</span>(<span cla=
ss=3D"cm-variable">steps</span><span class=3D"cm-operator">=3D</span><span =
class=3D"cm-number">30</span>)</span></pre></div><div style=3D"position: re=
lative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><d=
iv class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px=
; width: 21px;">51</div></div><pre class=3D" CodeMirror-line " role=3D"pres=
entation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span=
 class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span clas=
s=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"=
cm-variable">train_size</span> <span class=3D"cm-operator">=3D</span> <span=
 class=3D"cm-builtin">int</span>(<span class=3D"cm-builtin">len</span>(<spa=
n class=3D"cm-variable">PriceData</span>) <span class=3D"cm-operator">*</sp=
an> <span class=3D"cm-number">0.8</span>)</span></pre></div><div style=3D"p=
osition: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left:=
 -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=
=3D"left: 0px; width: 21px;">52</div></div><pre class=3D" CodeMirror-line "=
 role=3D"presentation"><span role=3D"presentation" style=3D"padding-right: =
0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </sp=
an><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-variable">train</span>, <span class=3D"cm-variable">test</s=
pan> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-variable">Pri=
ceData</span>[<span class=3D"cm-number">0</span>:<span class=3D"cm-variable=
">train_size</span>], <span class=3D"cm-variable">PriceData</span>[<span cl=
ass=3D"cm-variable">train_size</span>:<span class=3D"cm-builtin">len</span>=
(<span class=3D"cm-variable">PriceData</span>)]</span></pre></div><div styl=
e=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D=
"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" s=
tyle=3D"left: 0px; width: 21px;">53</div></div><pre class=3D" CodeMirror-li=
ne " role=3D"presentation"><span role=3D"presentation" style=3D"padding-rig=
ht: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    =
</span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </spa=
n><span class=3D"cm-variable">model_train</span> <span class=3D"cm-operator=
">=3D</span> <span class=3D"cm-variable">ARIMA</span>(<span class=3D"cm-var=
iable">train</span>[<span class=3D"cm-string">'Low'</span>], <span class=3D=
"cm-variable">order</span><span class=3D"cm-operator">=3D</span>(<span clas=
s=3D"cm-number">1</span>, <span class=3D"cm-number">1</span>, <span class=
=3D"cm-number">1</span>))</span></pre></div><div style=3D"position: relativ=
e;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div cl=
ass=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; wid=
th: 21px;">54</div></div><pre class=3D" CodeMirror-line " role=3D"presentat=
ion"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span clas=
s=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"=
cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-va=
riable">model_train_fit</span> <span class=3D"cm-operator">=3D</span> <span=
 class=3D"cm-variable">model_train</span>.<span class=3D"cm-property">fit</=
span>()</span></pre></div><div style=3D"position: relative;"><div class=3D"=
CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-=
linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">55</div=
></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D=
"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-variable">test_fore=
cast</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-variab=
le">model_train_fit</span>.<span class=3D"cm-property">get_forecast</span>(=
<span class=3D"cm-variable">steps</span><span class=3D"cm-operator">=3D</sp=
an><span class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">test</=
span>))</span></pre></div><div style=3D"position: relative;"><div class=3D"=
CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-=
linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">56</div=
></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D=
"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-variable">test_fore=
cast_series</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm=
-variable">pd</span>.<span class=3D"cm-property">Series</span>(<span class=
=3D"cm-variable">test_forecast</span>.<span class=3D"cm-property">predicted=
_mean</span>, <span class=3D"cm-variable">index</span><span class=3D"cm-ope=
rator">=3D</span><span class=3D"cm-variable">test</span>.<span class=3D"cm-=
property">index</span>)</span></pre></div><div style=3D"position: relative;=
"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div clas=
s=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width=
: 21px;">57</div></div><pre class=3D" CodeMirror-line " role=3D"presentatio=
n"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-var=
iable">mse</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-=
variable">mean_squared_error</span>(<span class=3D"cm-variable">test</span>=
[<span class=3D"cm-string">'Low'</span>], <span class=3D"cm-variable">test_=
forecast_series</span>)</span></pre></div><div style=3D"position: relative;=
"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div clas=
s=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width=
: 21px;">58</div></div><pre class=3D" CodeMirror-line " role=3D"presentatio=
n"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-var=
iable">rmse</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm=
-variable">mse</span><span class=3D"cm-operator">**</span><span class=3D"cm=
-number">0.5</span></span></pre></div><div style=3D"position: relative;"><d=
iv class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D=
"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21=
px;">59</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><=
span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab=
" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variable=
">model2</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-va=
riable">ARIMA</span>(<span class=3D"cm-variable">PriceData</span>[<span cla=
ss=3D"cm-string">'High'</span>], <span class=3D"cm-variable">order</span><s=
pan class=3D"cm-operator">=3D</span>(<span class=3D"cm-number">1</span>, <s=
pan class=3D"cm-number">1</span>, <span class=3D"cm-number">1</span>))</spa=
n></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-g=
utter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber C=
odeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">60</div></div><pre =
class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentatio=
n" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentat=
ion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-variable">model_fit2</span> <spa=
n class=3D"cm-operator">=3D</span> <span class=3D"cm-variable">model2</span=
>.<span class=3D"cm-property">fit</span>()</span></pre></div><div style=3D"=
position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left=
: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=
=3D"left: 0px; width: 21px;">61</div></div><pre class=3D" CodeMirror-line "=
 role=3D"presentation"><span role=3D"presentation" style=3D"padding-right: =
0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </sp=
an><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><s=
pan class=3D"cm-variable">forecast2</span> <span class=3D"cm-operator">=3D<=
/span> <span class=3D"cm-variable">model_fit2</span>.<span class=3D"cm-prop=
erty">get_forecast</span>(<span class=3D"cm-variable">steps</span><span cla=
ss=3D"cm-operator">=3D</span><span class=3D"cm-number">30</span>)</span></p=
re></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gutter=
-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMi=
rror-gutter-elt" style=3D"left: 0px; width: 21px;">62</div></div><pre class=
=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" st=
yle=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" =
cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-te=
xt=3D"	">    </span><span class=3D"cm-variable">train_size2</span> <span cl=
ass=3D"cm-operator">=3D</span> <span class=3D"cm-builtin">int</span>(<span =
class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">PriceData</span=
>) <span class=3D"cm-operator">*</span> <span class=3D"cm-number">0.8</span=
>)</span></pre></div><div style=3D"position: relative;"><div class=3D"CodeM=
irror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linen=
umber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">63</div></di=
v><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"pres=
entation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"pr=
esentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"present=
ation" cm-text=3D"	">    </span><span class=3D"cm-variable">train2</span>, =
<span class=3D"cm-variable">test2</span> <span class=3D"cm-operator">=3D</s=
pan> <span class=3D"cm-variable">PriceData</span>[<span class=3D"cm-number"=
>0</span>:<span class=3D"cm-variable">train_size2</span>], <span class=3D"c=
m-variable">PriceData</span>[<span class=3D"cm-variable">train_size2</span>=
:<span class=3D"cm-builtin">len</span>(<span class=3D"cm-variable">PriceDat=
a</span>)]</span></pre></div><div style=3D"position: relative;"><div class=
=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMir=
ror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">64<=
/div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span rol=
e=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" r=
ole=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variable">mode=
l_train2</span> <span class=3D"cm-operator">=3D</span> <span class=3D"cm-va=
riable">ARIMA</span>(<span class=3D"cm-variable">train2</span>[<span class=
=3D"cm-string">'High'</span>], <span class=3D"cm-variable">order</span><spa=
n class=3D"cm-operator">=3D</span>(<span class=3D"cm-number">1</span>, <spa=
n class=3D"cm-number">1</span>, <span class=3D"cm-number">1</span>))</span>=
</pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gut=
ter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Cod=
eMirror-gutter-elt" style=3D"left: 0px; width: 21px;">65</div></div><pre cl=
ass=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation"=
 style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-variable">model_train_fit2</span> =
<span class=3D"cm-operator">=3D</span> <span class=3D"cm-variable">model_tr=
ain2</span>.<span class=3D"cm-property">fit</span>()</span></pre></div><div=
 style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" sty=
le=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-e=
lt" style=3D"left: 0px; width: 21px;">66</div></div><pre class=3D" CodeMirr=
or-line " role=3D"presentation"><span role=3D"presentation" style=3D"paddin=
g-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"=
>    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    =
</span><span class=3D"cm-variable">test_forecast2</span> <span class=3D"cm-=
operator">=3D</span> <span class=3D"cm-variable">model_train_fit2</span>.<s=
pan class=3D"cm-property">get_forecast</span>(<span class=3D"cm-variable">s=
teps</span><span class=3D"cm-operator">=3D</span><span class=3D"cm-builtin"=
>len</span>(<span class=3D"cm-variable">test2</span>))</span></pre></div><d=
iv style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" s=
tyle=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter=
-elt" style=3D"left: 0px; width: 21px;">67</div></div><pre class=3D" CodeMi=
rror-line " role=3D"presentation"><span role=3D"presentation" style=3D"padd=
ing-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"=
	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">  =
  </span><span class=3D"cm-variable">test_forecast_series2</span> <span cla=
ss=3D"cm-operator">=3D</span> <span class=3D"cm-variable">pd</span>.<span c=
lass=3D"cm-property">Series</span>(<span class=3D"cm-variable">test_forecas=
t2</span>.<span class=3D"cm-property">predicted_mean</span>, <span class=3D=
"cm-variable">index</span><span class=3D"cm-operator">=3D</span><span class=
=3D"cm-variable">test2</span>.<span class=3D"cm-property">index</span>)</sp=
an></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-=
gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber =
CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">68</div></div><pre=
 class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentati=
on" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presenta=
tion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation"=
 cm-text=3D"	">    </span><span class=3D"cm-variable">mse2</span> <span cla=
ss=3D"cm-operator">=3D</span> <span class=3D"cm-variable">mean_squared_erro=
r</span>(<span class=3D"cm-variable">test2</span>[<span class=3D"cm-string"=
>'High'</span>], <span class=3D"cm-variable">test_forecast_series2</span>)<=
/span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirr=
or-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumb=
er CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">69</div></div><=
pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"present=
ation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"prese=
ntation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentati=
on" cm-text=3D"	">    </span><span class=3D"cm-variable">rmse2</span> <span=
 class=3D"cm-operator">=3D</span> <span class=3D"cm-variable">mse2</span><s=
pan class=3D"cm-operator">**</span><span class=3D"cm-number">0.5</span></sp=
an></pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-=
gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber =
CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">70</div></div><pre=
 class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentati=
on" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presenta=
tion" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation"=
 cm-text=3D"	">    </span><span class=3D"cm-variable">plt</span>.<span clas=
s=3D"cm-property">figure</span>(<span class=3D"cm-variable">figsize</span><=
span class=3D"cm-operator">=3D</span>(<span class=3D"cm-number">14</span>,<=
span class=3D"cm-number">7</span>))</span></pre></div><div style=3D"positio=
n: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px=
;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left=
: 0px; width: 21px;">71</div></div><pre class=3D" CodeMirror-line " role=3D=
"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;">=
<span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span=
 class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span clas=
s=3D"cm-variable">plt</span>.<span class=3D"cm-property">plot</span>(<span =
class=3D"cm-variable">train</span>[<span class=3D"cm-string">'Low'</span>],=
 <span class=3D"cm-variable">label</span><span class=3D"cm-operator">=3D</s=
pan><span class=3D"cm-string">'Training Low'</span>, <span class=3D"cm-vari=
able">color</span><span class=3D"cm-operator">=3D</span><span class=3D"cm-s=
tring">'red'</span>)</span></pre></div><div style=3D"position: relative;"><=
div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=
=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width:=
 21px;">72</div></div><pre class=3D" CodeMirror-line " role=3D"presentation=
"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span class=
=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"c=
m-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-var=
iable">plt</span>.<span class=3D"cm-property">plot</span>(<span class=3D"cm=
-variable">test</span>[<span class=3D"cm-string">'Low'</span>], <span class=
=3D"cm-variable">label</span><span class=3D"cm-operator">=3D</span><span cl=
ass=3D"cm-string">'Actual Low'</span>, <span class=3D"cm-variable">color</s=
pan><span class=3D"cm-operator">=3D</span><span class=3D"cm-string">'red'</=
span>)</span></pre></div><div style=3D"position: relative;"><div class=3D"C=
odeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-l=
inenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">73</div>=
</div><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"=
presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"p=
resentation" cm-text=3D"	">    </span><span class=3D"cm-variable">plt</span=
>.<span class=3D"cm-property">plot</span>(<span class=3D"cm-variable">test_=
forecast_series</span>, <span class=3D"cm-variable">label</span><span class=
=3D"cm-operator">=3D</span><span class=3D"cm-string">'Forecasted Low'</span=
>, <span class=3D"cm-variable">color</span><span class=3D"cm-operator">=3D<=
/span><span class=3D"cm-string">'yellow'</span>)</span></pre></div><div sty=
le=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=
=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt=
" style=3D"left: 0px; width: 21px;">74</div></div><pre class=3D" CodeMirror=
-line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-=
right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"> =
   </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </=
span><span class=3D"cm-variable">plt</span>.<span class=3D"cm-property">plo=
t</span>(<span class=3D"cm-variable">train2</span>[<span class=3D"cm-string=
">'High'</span>], <span class=3D"cm-variable">label</span><span class=3D"cm=
-operator">=3D</span><span class=3D"cm-string">'Training High'</span>, <spa=
n class=3D"cm-variable">color</span><span class=3D"cm-operator">=3D</span><=
span class=3D"cm-string">'blue'</span>)</span></pre></div><div style=3D"pos=
ition: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -=
34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"=
left: 0px; width: 21px;">75</div></div><pre class=3D" CodeMirror-line " rol=
e=3D"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1p=
x;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><=
span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span =
class=3D"cm-variable">plt</span>.<span class=3D"cm-property">plot</span>(<s=
pan class=3D"cm-variable">test2</span>[<span class=3D"cm-string">'High'</sp=
an>], <span class=3D"cm-variable">label</span><span class=3D"cm-operator">=
=3D</span><span class=3D"cm-string">'Actual High'</span>, <span class=3D"cm=
-variable">color</span><span class=3D"cm-operator">=3D</span><span class=3D=
"cm-string">'blue'</span>)</span></pre></div><div style=3D"position: relati=
ve;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div c=
lass=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; wi=
dth: 21px;">76</div></div><pre class=3D" CodeMirror-line " role=3D"presenta=
tion"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span cla=
ss=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D=
"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-v=
ariable">plt</span>.<span class=3D"cm-property">plot</span>(<span class=3D"=
cm-variable">test_forecast_series2</span>, <span class=3D"cm-variable">labe=
l</span><span class=3D"cm-operator">=3D</span><span class=3D"cm-string">'Fo=
recasted High'</span>, <span class=3D"cm-variable">color</span><span class=
=3D"cm-operator">=3D</span><span class=3D"cm-string">'green'</span>)</span>=
</pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gut=
ter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Cod=
eMirror-gutter-elt" style=3D"left: 0px; width: 21px;">77</div></div><pre cl=
ass=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation"=
 style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-variable">plt</span>.<span class=
=3D"cm-property">fill_between</span>(<span class=3D"cm-variable">test</span=
>.<span class=3D"cm-property">index</span>, <span class=3D"cm-variable">tes=
t_forecast</span>.<span class=3D"cm-property">conf_int</span>().<span class=
=3D"cm-property">iloc</span>[:, <span class=3D"cm-number">0</span>],</span>=
</pre></div><div style=3D"position: relative;"><div class=3D"CodeMirror-gut=
ter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Cod=
eMirror-gutter-elt" style=3D"left: 0px; width: 21px;">78</div></div><pre cl=
ass=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation"=
 style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" role=3D"presentatio=
n" cm-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm=
-text=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=
=3D"	">    </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	=
">    </span> <span class=3D"cm-variable">test_forecast</span>.<span class=
=3D"cm-property">conf_int</span>().<span class=3D"cm-property">iloc</span>[=
:, <span class=3D"cm-number">1</span>],<span class=3D"cm-variable">color</s=
pan><span class=3D"cm-operator">=3D</span><span class=3D"cm-string">'k'</sp=
an>, <span class=3D"cm-variable">alpha</span><span class=3D"cm-operator">=
=3D</span><span class=3D"cm-number">.15</span>)</span></pre></div><div styl=
e=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D=
"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" s=
tyle=3D"left: 0px; width: 21px;">79</div></div><pre class=3D" CodeMirror-li=
ne " role=3D"presentation"><span role=3D"presentation" style=3D"padding-rig=
ht: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    =
</span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </spa=
n><span class=3D"cm-variable">plt</span>.<span class=3D"cm-property">fill_b=
etween</span>(<span class=3D"cm-variable">test2</span>.<span class=3D"cm-pr=
operty">index</span>, <span class=3D"cm-variable">test_forecast2</span>.<sp=
an class=3D"cm-property">conf_int</span>().<span class=3D"cm-property">iloc=
</span>[:, <span class=3D"cm-number">0</span>],</span></pre></div><div styl=
e=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D=
"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" s=
tyle=3D"left: 0px; width: 21px;">80</div></div><pre class=3D" CodeMirror-li=
ne " role=3D"presentation"><span role=3D"presentation" style=3D"padding-rig=
ht: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    =
</span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </spa=
n><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><sp=
an class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span> <span c=
lass=3D"cm-variable">test_forecast2</span>.<span class=3D"cm-property">conf=
_int</span>().<span class=3D"cm-property">iloc</span>[:, <span class=3D"cm-=
number">1</span>],<span class=3D"cm-variable">color</span><span class=3D"cm=
-operator">=3D</span><span class=3D"cm-string">'k'</span>, <span class=3D"c=
m-variable">alpha</span><span class=3D"cm-operator">=3D</span><span class=
=3D"cm-number">.15</span>)</span></pre></div><div style=3D"position: relati=
ve;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div c=
lass=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; wi=
dth: 21px;">81</div></div><pre class=3D" CodeMirror-line " role=3D"presenta=
tion"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span cla=
ss=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D=
"cm-tab" role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-v=
ariable">plt</span>.<span class=3D"cm-property">title</span>(<span class=3D=
"cm-string">'ARIMA Model Evaluation'</span>)</span></pre></div><div style=
=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"=
left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" st=
yle=3D"left: 0px; width: 21px;">82</div></div><pre class=3D" CodeMirror-lin=
e " role=3D"presentation"><span role=3D"presentation" style=3D"padding-righ=
t: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    <=
/span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span=
><span class=3D"cm-variable">plt</span>.<span class=3D"cm-property">xlabel<=
/span>(<span class=3D"cm-string">'Day'</span>)</span></pre></div><div style=
=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"=
left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" st=
yle=3D"left: 0px; width: 21px;">83</div></div><pre class=3D" CodeMirror-lin=
e " role=3D"presentation"><span role=3D"presentation" style=3D"padding-righ=
t: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    <=
/span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </span=
><span class=3D"cm-variable">plt</span>.<span class=3D"cm-property">ylabel<=
/span>(<span class=3D"cm-string">'Price'</span>)</span></pre></div><div sty=
le=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=
=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt=
" style=3D"left: 0px; width: 21px;">84</div></div><pre class=3D" CodeMirror=
-line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-=
right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"> =
   </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </=
span><span class=3D"cm-variable">plt</span>.<span class=3D"cm-property">leg=
end</span>()</span></pre></div><div style=3D"position: relative;"><div clas=
s=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMi=
rror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">85=
</div></div><pre class=3D" CodeMirror-line " role=3D"presentation"><span ro=
le=3D"presentation" style=3D"padding-right: 0.1px;"><span class=3D"cm-tab" =
role=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-tab" role=
=3D"presentation" cm-text=3D"	">    </span><span class=3D"cm-variable">plt<=
/span>.<span class=3D"cm-property">show</span>()</span></pre></div><div sty=
le=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=
=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt=
" style=3D"left: 0px; width: 21px;">86</div></div><pre class=3D" CodeMirror=
-line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-=
right: 0.1px;"><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	"> =
   </span><span class=3D"cm-tab" role=3D"presentation" cm-text=3D"	">    </=
span><span class=3D"cm-keyword">return</span> [<span class=3D"cm-variable">=
rmse</span>, <span class=3D"cm-variable">rmse2</span>]</span></pre></div><d=
iv style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" s=
tyle=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter=
-elt" style=3D"left: 0px; width: 21px;">87</div></div><pre class=3D" CodeMi=
rror-line " role=3D"presentation"><span role=3D"presentation" style=3D"padd=
ing-right: 0.1px;">    </span></pre></div><div style=3D"position: relative;=
"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><div clas=
s=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px; width=
: 21px;">88</div></div><pre class=3D" CodeMirror-line " role=3D"presentatio=
n"><span role=3D"presentation" style=3D"padding-right: 0.1px;">    </span><=
/pre></div></div></div></div></div></div><div style=3D"position: absolute; =
height: 33px; width: 1px; border-bottom: 17px solid transparent; top: 1507p=
x;"></div><div class=3D"CodeMirror-gutters" style=3D"height: 1557px; left: =
0px;"><div class=3D"CodeMirror-gutter CodeMirror-linenumbers" style=3D"widt=
h: 33px;"></div></div></div></div></div></div></div><div class=3D"output_wr=
apper"><div class=3D"out_prompt_overlay prompt" title=3D"click to scroll ou=
tput; double click to hide"></div><div class=3D"output"></div><div class=3D=
"btn btn-default output_collapsed" title=3D"click to expand output" style=
=3D"display: none;">. . .</div></div></div><div class=3D"cell code_cell ren=
dered unselected" tabindex=3D"2"><div class=3D"input"><div class=3D"prompt_=
container"><div class=3D"prompt input_prompt"><bdi>In</bdi>&nbsp;[14]:</div=
><div class=3D"run_this_cell" title=3D"Run this cell"><i class=3D"fa-step-f=
orward fa"></i></div></div><div class=3D"inner_cell"><div class=3D"ctb_hide=
show"><div class=3D"celltoolbar"></div></div><div class=3D"input_area" aria=
-label=3D"Edit code here"><div class=3D"CodeMirror cm-s-ipython"><div style=
=3D"overflow: hidden; position: relative; width: 3px; height: 0px; top: 22.=
6px; left: 612px;"><textarea autocorrect=3D"off" autocapitalize=3D"off" spe=
llcheck=3D"false" tabindex=3D"0" style=3D"position: absolute; bottom: -1em;=
 padding: 0px; width: 1000px; height: 1em; outline: none;"></textarea></div=
><div class=3D"CodeMirror-vscrollbar" tabindex=3D"-1" cm-not-content=3D"tru=
e"><div style=3D"min-width: 1px; height: 0px;"></div></div><div class=3D"Co=
deMirror-hscrollbar" tabindex=3D"-1" cm-not-content=3D"true" style=3D"displ=
ay: block; right: 0px; left: 34px;"><div style=3D"height: 100%; min-height:=
 1px; width: 653.588px;"></div></div><div class=3D"CodeMirror-scrollbar-fil=
ler" cm-not-content=3D"true"></div><div class=3D"CodeMirror-gutter-filler" =
cm-not-content=3D"true"></div><div class=3D"CodeMirror-scroll" tabindex=3D"=
-1" draggable=3D"false"><div class=3D"CodeMirror-sizer" style=3D"margin-lef=
t: 34px; min-width: 653.588px; margin-bottom: -17px; border-right-width: 33=
px; min-height: 45px; padding-right: 0px; padding-bottom: 17px;"><div style=
=3D"position: relative; top: 0px;"><div class=3D"CodeMirror-lines" role=3D"=
presentation"><div role=3D"presentation" style=3D"position: relative; outli=
ne: none;"><div class=3D"CodeMirror-measure"><pre class=3D"CodeMirror-line-=
like">x</pre></div><div class=3D"CodeMirror-measure"></div><div style=3D"po=
sition: relative; z-index: 1;"><div class=3D"CodeMirror-selected" style=3D"=
position: absolute; left: 4px; top: 0px; width: 645.588px; height: 17px;"><=
/div><div class=3D"CodeMirror-selected" style=3D"position: absolute; left: =
4px; top: 17px; width: 646.588px; height: 17px;"></div></div><div class=3D"=
CodeMirror-cursors" style=3D""></div><div class=3D"CodeMirror-code" role=3D=
"presentation"><div style=3D"position: relative;"><div class=3D"CodeMirror-=
gutter-wrapper" style=3D"left: 30.8px;"><div class=3D"CodeMirror-linenumber=
 CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">1</div></div><pre=
 class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentati=
on" style=3D"padding-right: 0.1px;"><span class=3D"cm-variable">w</span><sp=
an class=3D"cm-operator">=3D</span><span class=3D"cm-variable">pred</span>(=
)</span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMi=
rror-gutter-wrapper" style=3D"left: 30.8px;"><div class=3D"CodeMirror-linen=
umber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">2</div></div=
><pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"prese=
ntation" style=3D"padding-right: 0.1px;"><span class=3D"cm-variable">gbpusd=
Data</span><span class=3D"cm-operator">=3D</span><span class=3D"cm-variable=
">w</span>.<span class=3D"cm-property">getData</span>(<span class=3D"cm-str=
ing">'https://www.investing.com/currencies/gbp-usd-historical-data'</span>)=
</span></pre></div></div></div></div></div></div><div style=3D"position: ab=
solute; height: 33px; width: 1px; border-bottom: 17px solid transparent; to=
p: 45px;"></div><div class=3D"CodeMirror-gutters" style=3D"height: 95px; le=
ft: 64.8px;"><div class=3D"CodeMirror-gutter CodeMirror-linenumbers" style=
=3D"width: 33px;"></div></div></div></div></div></div></div><div class=3D"o=
utput_wrapper"><div class=3D"out_prompt_overlay prompt" title=3D"click to s=
croll output; double click to hide"></div><div class=3D"output"></div><div =
class=3D"btn btn-default output_collapsed" title=3D"click to expand output"=
 style=3D"display: none;">. . .</div></div></div><div class=3D"cell code_ce=
ll rendered unselected" tabindex=3D"2"><div class=3D"input"><div class=3D"p=
rompt_container"><div class=3D"prompt input_prompt"><bdi>In</bdi>&nbsp;[15]=
:</div><div class=3D"run_this_cell" title=3D"Run this cell"><i class=3D"fa-=
step-forward fa"></i></div></div><div class=3D"inner_cell"><div class=3D"ct=
b_hideshow"><div class=3D"celltoolbar"></div></div><div class=3D"input_area=
" aria-label=3D"Edit code here"><div class=3D"CodeMirror cm-s-ipython"><div=
 style=3D"overflow: hidden; position: relative; width: 3px; height: 0px; to=
p: 5.60001px; left: 168.863px;"><textarea autocorrect=3D"off" autocapitaliz=
e=3D"off" spellcheck=3D"false" tabindex=3D"0" style=3D"position: absolute; =
bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: none;"></t=
extarea></div><div class=3D"CodeMirror-vscrollbar" tabindex=3D"-1" cm-not-c=
ontent=3D"true"><div style=3D"min-width: 1px; height: 0px;"></div></div><di=
v class=3D"CodeMirror-hscrollbar" tabindex=3D"-1" cm-not-content=3D"true"><=
div style=3D"height: 100%; min-height: 1px; width: 0px;"></div></div><div c=
lass=3D"CodeMirror-scrollbar-filler" cm-not-content=3D"true"></div><div cla=
ss=3D"CodeMirror-gutter-filler" cm-not-content=3D"true"></div><div class=3D=
"CodeMirror-scroll" tabindex=3D"-1"><div class=3D"CodeMirror-sizer" style=
=3D"margin-left: 34px; min-width: 137.863px; margin-bottom: -17px; border-r=
ight-width: 33px; min-height: 28px; padding-right: 0px; padding-bottom: 0px=
;"><div style=3D"position: relative; top: 0px;"><div class=3D"CodeMirror-li=
nes" role=3D"presentation"><div role=3D"presentation" style=3D"position: re=
lative; outline: none;"><div class=3D"CodeMirror-measure"><pre class=3D"Cod=
eMirror-line-like">x</pre></div><div class=3D"CodeMirror-measure"></div><di=
v style=3D"position: relative; z-index: 1;"><div class=3D"CodeMirror-select=
ed" style=3D"position: absolute; left: 4px; top: 0px; width: 130.863px; hei=
ght: 17px;"></div></div><div class=3D"CodeMirror-cursors" style=3D""></div>=
<div class=3D"CodeMirror-code" role=3D"presentation"><div style=3D"position=
: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;=
"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left:=
 0px; width: 21px;">1</div></div><pre class=3D" CodeMirror-line " role=3D"p=
resentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><s=
pan class=3D"cm-builtin">print</span>(<span class=3D"cm-variable">gbpusdDat=
a</span>)</span></pre></div></div></div></div></div></div><div style=3D"pos=
ition: absolute; height: 33px; width: 1px; border-bottom: 0px solid transpa=
rent; top: 28px;"></div><div class=3D"CodeMirror-gutters" style=3D"height: =
61px; left: 0px;"><div class=3D"CodeMirror-gutter CodeMirror-linenumbers" s=
tyle=3D"width: 33px;"></div></div></div></div></div></div></div><div class=
=3D"output_wrapper"><div class=3D"out_prompt_overlay prompt" title=3D"click=
 to unscroll output; double click to hide"></div><div class=3D"output outpu=
t_scroll"><div class=3D"output_area"><div class=3D"run_this_cell"></div><di=
v class=3D"prompt"></div><div class=3D"output_subarea output_text output_st=
ream output_stdout" dir=3D"auto"><pre>          Date   Price    Open    Hig=
h     Low
0   01-24-2024  1.2723  1.2688  1.2776  1.2677
1   01-25-2024  1.2708  1.2721  1.2744  1.2680
2   01-26-2024  1.2702  1.2710  1.2759  1.2674
3   01-29-2024  1.2707  1.2697  1.2720  1.2661
4   01-30-2024  1.2697  1.2710  1.2723  1.2639
5   01-31-2024  1.2685  1.2699  1.2752  1.2657
6   02-01-2024  1.2742  1.2687  1.2757  1.2624
7   02-02-2024  1.2630  1.2744  1.2774  1.2613
8   02-05-2024  1.2532  1.2633  1.2644  1.2517
9   02-06-2024  1.2597  1.2536  1.2605  1.2529
10  02-07-2024  1.2625  1.2598  1.2643  1.2591
11  02-08-2024  1.2616  1.2626  1.2640  1.2571
12  02-09-2024  1.2619  1.2622  1.2644  1.2598
13  02-12-2024  1.2626  1.2625  1.2656  1.2605
14  02-13-2024  1.2589  1.2630  1.2685  1.2572
15  02-14-2024  1.2565  1.2590  1.2613  1.2534
16  02-15-2024  1.2600  1.2565  1.2603  1.2541
17  02-16-2024  1.2598  1.2600  1.2626  1.2550
18  02-19-2024  1.2593  1.2603  1.2631  1.2582
19  02-20-2024  1.2618  1.2591  1.2670  1.2578
20  02-21-2024  1.2634  1.2622  1.2643  1.2601
21  02-22-2024  1.2659  1.2638  1.2711  1.2610
22  02-23-2024  1.2679  1.2659  1.2702  1.2648
</pre></div></div></div><div class=3D"btn btn-default output_collapsed" tit=
le=3D"click to expand output" style=3D"display: none;">. . .</div></div></d=
iv><div class=3D"cell code_cell rendered unselected" tabindex=3D"2"><div cl=
ass=3D"input"><div class=3D"prompt_container"><div class=3D"prompt input_pr=
ompt"><bdi>In</bdi>&nbsp;[18]:</div><div class=3D"run_this_cell" title=3D"R=
un this cell"><i class=3D"fa-step-forward fa"></i></div></div><div class=3D=
"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"celltoolbar"></div><=
/div><div class=3D"input_area" aria-label=3D"Edit code here"><div class=3D"=
CodeMirror cm-s-ipython"><div style=3D"overflow: hidden; position: relative=
; width: 3px; height: 0px; top: 22.6px; left: 245.844px;"><textarea autocor=
rect=3D"off" autocapitalize=3D"off" spellcheck=3D"false" tabindex=3D"0" sty=
le=3D"position: absolute; bottom: -1em; padding: 0px; width: 1000px; height=
: 1em; outline: none;"></textarea></div><div class=3D"CodeMirror-vscrollbar=
" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"min-width: 1px; hei=
ght: 0px;"></div></div><div class=3D"CodeMirror-hscrollbar" tabindex=3D"-1"=
 cm-not-content=3D"true"><div style=3D"height: 100%; min-height: 1px; width=
: 0px;"></div></div><div class=3D"CodeMirror-scrollbar-filler" cm-not-conte=
nt=3D"true"></div><div class=3D"CodeMirror-gutter-filler" cm-not-content=3D=
"true"></div><div class=3D"CodeMirror-scroll" tabindex=3D"-1" draggable=3D"=
false"><div class=3D"CodeMirror-sizer" style=3D"margin-left: 34px; min-widt=
h: 261.025px; margin-bottom: -17px; border-right-width: 33px; min-height: 4=
5px; padding-right: 0px; padding-bottom: 0px;"><div style=3D"position: rela=
tive; top: 0px;"><div class=3D"CodeMirror-lines" role=3D"presentation"><div=
 role=3D"presentation" style=3D"position: relative; outline: none;"><div cl=
ass=3D"CodeMirror-measure"><pre class=3D"CodeMirror-line-like">x</pre></div=
><div class=3D"CodeMirror-measure"></div><div style=3D"position: relative; =
z-index: 1;"><div class=3D"CodeMirror-selected" style=3D"position: absolute=
; left: 4px; top: 0px; width: 580px; height: 17px;"></div><div class=3D"Cod=
eMirror-selected" style=3D"position: absolute; left: 4px; top: 17px; width:=
 207.844px; height: 17px;"></div></div><div class=3D"CodeMirror-cursors" st=
yle=3D""></div><div class=3D"CodeMirror-code" role=3D"presentation"><div st=
yle=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=
=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt=
" style=3D"left: 0px; width: 21px;">1</div></div><pre class=3D" CodeMirror-=
line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-r=
ight: 0.1px;"><span class=3D"cm-variable">warnings</span>.<span class=3D"cm=
-property">filterwarnings</span>(<span class=3D"cm-string">"ignore"</span>)=
</span></pre></div><div style=3D"position: relative;"><div class=3D"CodeMir=
ror-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenum=
ber CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">2</div></div><=
pre class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"present=
ation" style=3D"padding-right: 0.1px;"><span class=3D"cm-variable">forcast<=
/span><span class=3D"cm-operator">=3D</span><span class=3D"cm-variable">w</=
span>.<span class=3D"cm-property">estim</span>(<span class=3D"cm-variable">=
gbpusdData</span>)</span></pre></div></div></div></div></div></div><div sty=
le=3D"position: absolute; height: 33px; width: 1px; border-bottom: 0px soli=
d transparent; top: 45px;"></div><div class=3D"CodeMirror-gutters" style=3D=
"height: 78px; left: 0px;"><div class=3D"CodeMirror-gutter CodeMirror-linen=
umbers" style=3D"width: 33px;"></div></div></div></div></div></div></div><d=
iv class=3D"output_wrapper"><div class=3D"out_prompt_overlay prompt" title=
=3D"click to scroll output; double click to hide"></div><div class=3D"outpu=
t"><div class=3D"output_area"><div class=3D"run_this_cell"></div><div class=
=3D"prompt"></div><div class=3D"output_subarea output_png" dir=3D"auto"><im=
g src=3D"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABJYAAAJuCAYAAADihog9=
AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMiwgaHR0cHM6Ly9tYXRwbG9=
0bGliLm9yZy8pXeV/AAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzdd1zV9RfH8ddlgw=
iK4N5K7pXmSlPLmSNtqaXmKE0rU1ta2rChpZa2bPzU0sxRmVk5UlOx3KZlZS5wIQ5QQTbce39/f=
OImggoIXpD38/H4PuB+73ecC1hw7jnnY7Hb7XZERERERERERESyycXZAYiIiIiIiIiISMGkxJKI=
iIiIiIiIiOSIEksiIiIiIiIiIpIjSiyJiIiIiIiIiEiOKLEkIiIiIiIiIiI5osSSiIiIiIiIiIj=
kiBJLIiIiIiIiIiKSI0osiYiIiIiIiIhIjiixJCIiIiIiIiIiOaLEkoiIiGTJu+++i8VioW7dup=
c9xmKxpNv8/Pxo2bIlCxYsyHDsZ599hsViYceOHY59L7/8MhaLBRcXF0JDQzOcExcXh5+fHxaLh=
YEDB2Yaw549e7BYLLi7uxMREZHl15cb986Jw4cPY7FY+Oyzz7J97vr167FYLKxfvz5Lx11uy8m9=
s2rgwIFUrlw5z64PcOLECV5++WV2796d4bm076uIiIjkDSWWREREJEtmz54NwF9//cXWrVsve9y=
9997L5s2b2bRpEx999BExMTE88MADfPnll1m+l6+vL3PmzMmw/6uvviIlJQV3d/fLnvu///0PgN=
TUVObOnZvle+bGvfO7N954g82bN2fYunbt6uzQrsmJEyd45ZVXMk0sPfzww2zevPn6ByUiIlJIK=
LEkIiIiV7Vjxw5+//13RwJi1qxZlz22VKlSNG/enBYtWvDAAw/w448/AvDxxx9n+X69e/fm888/=
x2azpds/a9YsevXqhYeHR6bnJSUlMX/+fBo0aEC5cuUcybDsyOm9C4Lg4GCaN2+eYQsKCnJ2aHm=
mfPnyNG/e3NlhiIiI3LCUWBIREZGrSkskTZ48mZYtW7Jw4ULi4+OzdG6lSpUICgri1KlTWb7f4M=
GDOXbsGKtXr3bs279/P7/88guDBw++7HlLly4lKiqKhx9+mIceeshxTnbk5N5Hjx6lX79+lCxZE=
k9PT2rVqsW0adMyJKdOnDjB/fffT9GiRfH396d3796cPHky02vu2LGDHj16EBAQgJeXF40aNWLx=
4sXZei3Z1bNnTypVqpQhboBmzZpx8803Ox5/8MEH3HbbbZQsWZIiRYpQr1493nrrLVJSUq54jyu=
1/lksFl5++WXH44MHDzJo0CCCg4Px8fGhXLlydO/enT179jiOWb9+PbfccgsAgwYNcrT3pV0ns1=
Y4m83GW2+9Rc2aNfH09KRkyZIMGDCA48ePpzuubdu21K1bl+3bt9O6dWt8fHyoWrUqkydPzvRrJ=
CIiUhgpsSQiIiJXlJCQwIIFC7jllluoW7cugwcP5sKFC3z11VdZOj86OpqzZ89y0003ZfmewcHB=
tG7dOl3F0ezZs6lcuTJ33HHHZc+bNWsWnp6ePPjggwwePBiLxXLF6qrcuPeZM2do2bIlP/30E6+=
++irLli2jffv2PP300zz++OOO4xISEmjfvj0//fQTkyZN4quvvqJ06dL07t07wzXXrVvHrbfeyv=
nz5/noo4/47rvvaNiwIb17976meUg2m43U1NQMW5rBgwdz9OhRfv7553Tn/fPPP2zbto1BgwY59=
h06dIgHHniAefPm8cMPPzBkyBCmTJnCsGHDchzfpU6cOEGJEiWYPHkyK1eu5IMPPsDNzY1mzZqx=
b98+AG6++WZH6+L48eMd7X0PP/zwZa87fPhwnnvuOTp06MCyZct49dVXWblyJS1btiQyMjLdsSd=
PnuTBBx+kX79+LFu2jC5dujBu3Di++OKLXHudIiIiBZpdRERE5Armzp1rB+wfffSR3W632y9cuG=
D39fW1t27dOsOxgH3EiBH2lJQUe3Jysn3//v32Hj162IsWLWrfsWNHumPnzJljB+zbt2937Hvpp=
ZfsgP3MmTP2OXPm2D09Pe1RUVH21NRUe5kyZewvv/yy3W6324sUKWJ/6KGH0l3v8OHDdhcXF3uf=
Pn0c+9q0aWMvUqSIPSYm5qqvM6f3Hjt2rB2wb926Nd31hg8fbrdYLPZ9+/bZ7Xa7febMmXbA/t1=
336U77pFHHrED9jlz5jj21axZ096oUSN7SkpKumO7detmL1OmjN1qtdrtdrt93bp1dsC+bt26K7=
62tOMutx07dsxut9vtKSkp9lKlStkfeOCBdOc/++yzdg8PD3tkZGSm17darfaUlBT73Llz7a6ur=
vazZ886nnvooYfslSpVcjwOCwvL8HrTAPaXXnrpsq8jNTXVnpycbA8ODraPHj3asX/79u2XvWba=
9zXN3r17HT+nF9u6dasdsD///POOfW3atMn0e1u7dm17p06dLhuniIhIYaKKJREREbmiWbNm4e3=
tTZ8+fQAz3Pq+++5j48aNHDhwIMPxH374Ie7u7nh4eHDTTTexYsUKFixYQOPGjbN13/vuuw8PDw=
/mz5/P8uXLOXny5BVXY5szZw42my1du9rgwYOJi4tj0aJFeXbvn3/+mdq1a9O0adN0+wcOHIjdb=
ndU/6xbt46iRYvSo0ePdMc98MAD6R4fPHiQf/75hwcffBAgXWXRnXfeSUREhKNaJ7vefPNNtm/f=
nmErVaoUAG5ubvTr148lS5YQHR0NgNVqZd68edx1112UKFHCca1du3bRo0cPSpQogaurK+7u7gw=
YMACr1cr+/ftzFN+lUlNTeeONN6hduzYeHh64ubnh4eHBgQMH2Lt3b46uuW7dOoAM38+mTZtSq1=
Yt1q5dm25/6dKlM3xv69evz5EjR3J0fxERkRuNEksiIiJyWQcPHiQkJISuXbtit9s5f/4858+f5=
9577wXIdDj2/fffz/bt29m0aRMff/wxRYsWpU+fPpkmoa6kSJEi9O7dm9mzZzNr1izat29PpUqV=
Mj3WZrPx2WefUbZsWRo3buyIs3379hQpUiTb7XDZuXdUVBRlypTJsL9s2bKO59M+piVwLla6dOl=
0j9NmUT399NO4u7un20aMGAGQoV0rq6pWrUqTJk0ybBevdDd48GASExNZuHAhAKtWrSIiIiJdG9=
zRo0dp3bo14eHhzJgxg40bN7J9+3Y++OADwLT95YYxY8YwYcIEevbsyffff8/WrVvZvn07DRo0y=
PE90r4fl/uepT2f5uJkWhpPT89ce40iIiIFnZuzAxAREZH8a/bs2djtdr7++mu+/vrrDM9//vnn=
vPbaa7i6ujr2BQUF0aRJEwBatGhBrVq1aNOmDaNHj+aHH37I1v0HDx7M//73P/744w/mz59/2eP=
WrFnjqCDJLBGwZcsW/v77b2rXrp3r9y5RogQREREZ9p84cQKAwMBAx3Hbtm3LcNylw7vTjh83bh=
x33313pvesUaNG1l5EDqRVX82ZM4dhw4YxZ84cypYtS8eOHR3HLF26lLi4OJYsWZIu4bZ79+6rX=
t/LywswK/hd7NKEDsAXX3zBgAEDeOONN9Ltj4yMpFixYtl4Vf9J+/mIiIigfPny6Z47ceKE4+sv=
IiIiWaOKJREREcmU1Wrl888/p1q1aqxbty7D9tRTTxEREcGKFSuueJ3WrVszYMAAfvzxRzZv3py=
tGFq0aMHgwYPp1asXvXr1uuxxs2bNwsXFhaVLl2aIc968eUDm1VW5ce877riDv//+m99++y3d/r=
lz52KxWGjXrh0A7dq148KFCyxbtizdcV9++WW6xzVq1CA4OJjff/890+qiJk2aULRo0Wy9luwaN=
GgQW7du5ZdffuH777/noYceSpc8TFtlzdPT07HPbrfz6aefXvXapUqVwsvLiz/++CPd/u+++y7D=
sRaLJd09AH788UfCw8PT7Us7JitVRLfffjtAhuHb27dvZ+/evVccDi8iIiIZqWJJREREMrVixQp=
OnDjBm2++Sdu2bTM8X7duXd5//31mzZpFt27drnitV199lUWLFjFhwgTWrFmTrTiu1sYWFRXFd9=
99R6dOnbjrrrsyPeadd95h7ty5TJo0KV3b17XeG2D06NHMnTuXrl27MnHiRCpVqsSPP/7Ihx9+y=
PDhwx2r4Q0YMIB33nmHAQMG8PrrrxMcHMzy5ctZtWpVhmt+/PHHdOnShU6dOjFw4EDKlSvH2bNn=
2bt3L7/99luWV+S71IEDB9iyZUuG/eXLl09XvdO3b1/GjBlD3759SUpKyjCPqEOHDnh4eNC3b1+=
effZZEhMTmTlzJufOnbtqDBaLhX79+jF79myqVatGgwYN2LZtW4YEG0C3bt347LPPqFmzJvXr12=
fnzp1MmTIlQ6VRtWrV8Pb2Zv78+dSqVQtfX1/Kli3raEe8WI0aNRg6dCjvvfceLi4udOnShcOHD=
zNhwgQqVKjA6NGjr/oaRERE5D+qWBIREZFMzZo1Cw8Pj3SzdS4WGBhIr169+OGHHxxzgS6nQoUK=
PPHEE6xdu5aQkJBcjfOLL74gKSnpisvcDx06lDNnzvD999/n6r3BtP5t2rSJ22+/nXHjxtGtWzd=
WrVrFW2+9xXvvvec4zsfHh59//pn27dszduxY7r33Xo4fP+6YZXSxdu3asW3bNooVK8aoUaNo37=
49w4cPZ82aNbRv3z7HsT7//PO0aNEiw/bRRx+lO87f359evXpx/Phxbr31VkdyLE3NmjX55ptvO=
HfuHHfffTdPPPEEDRs25N13381SHNOmTaNfv3689dZb3HXXXWzevDnTNskZM2bQr18/Jk2aRPfu=
3Vm2bBlLliyhWrVq6Y7z8fFh9uzZREVF0bFjR2655RY++eSTy95/5syZTJ48meXLl9OtWzdeeOE=
FOnbsyKZNmzJtpRQREZHLs9jtdruzgxARERERERERkYJHFUsiIiIiIiIiIpIjSiyJiIiIiIiIiE=
iOKLEkIiIiIiIiIiI5osSSiIiIiIiIiIjkiBJLIiIiIiIiIiKSI0osiYiIiIiIiIhIjrg5O4CCy=
mazceLECYoWLYrFYnF2OCIiIiIiIiIiucJut3PhwgXKli2Li8uVa5KUWMqhEydOUKFCBWeHISIi=
IiIiIiKSJ44dO0b58uWveIwSSzlUtGhRwHyR/fz8nByNiIiIiIiIiEjuiImJoUKFCo7cx5UosZR=
Dae1vfn5+SiyJiIiIiIiIyA0nK6N/NLxbRERERERERERyRIklERERERERERHJESWWRERERERERE=
QkRzRjSURERERERMQJrFYrKSkpzg5DCiFXV1fc3NyyNEPpapRYEhEREREREbnOYmNjOX78OHa73=
dmhSCHl4+NDmTJl8PDwuKbrKLEkIiIiIiIich1ZrVaOHz+Oj48PQUFBuVI1IpJVdrud5ORkzpw5=
Q1hYGMHBwbi45HxSkhJLIiIiIiIiItdRSkoKdrudoKAgvL29nR2OFELe3t64u7tz5MgRkpOT8fL=
yyvG1NLxbRERERERExAlUqSTOdC1VSumukytXERERERERERGRQkeJJRERERERERERyREllkRERE=
RERETEKdq2bcuoUaOyfPzhw4exWCzs3r07z2KS7FFiSURERERERESuyGKxXHEbOHBgjq67ZMkSX=
n311SwfX6FCBSIiIqhbt26O7pdVSmBlnVaFExEREREREZErioiIcHy+aNEiXnzxRfbt2+fYd+nq=
dikpKbi7u1/1ugEBAdmKw9XVldKlS2frHMlbqlgSERERERERcSa7HeLinLPZ7VkKsXTp0o7N398=
fi8XieJyYmEixYsVYvHgxbdu2xcvLiy+++IKoqCj69u1L+fLl8fHxoV69eixYsCDddS9thatcuT=
JvvPEGgwcPpmjRolSsWJFPPvnE8fyllUTr16/HYrGwdu1amjRpgo+PDy1btkyX9AJ47bXXKFmyJ=
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
TO89dZbHDp0iA8++IAVK1aku3/16tWZN28ee/fuZevWrTz44IN4e3uTmppKQkICSUlJAFetUoqJ=
ieH3339Ptx09epShQ4dy/PhxRo8ezb59+/j+++957bXXGDlypON6aXOWFixY4Jil1KpVK3bv3l1=
o5yuBEksiIiIiIiIichWzZs2iffv2+Pv7Z3junnvuYffu3fz222+0bduWr776imXLltGwYUNuv/=
12tm7d6jh24sSJHD58mGrVqhEUFASYaqEPP/yQDz74gAYNGrBt2zaefvrpdPeYPXs2586do1GjR=
vTv358RI0YQFBREamoqAO7u7ll6HSEhITRv3jzd9uqrr1KuXDmWLl3Kjh07aNq0KSNHjuShhx5i=
7Nix6c6/7bbbsFqtjiRS8eLFqVWrFkFBQdSsWTPrX9AbiMV+pWXZ5LJiYmLw9/cnOjoaPz8/Z4c=
jIiIiIiIiBURiYiJhYWFUqVIFLy8vZ4dTYNhsNscqbzabDRcXF1xdXZ0dVgZprX4+Pj5XHBjubF=
f6OcxOzkPDu0VEREREREQk37LZbFitVpKTkx0JpaxWKEneU2JJRERERERERPIdu93uqFCyWq1KK=
OVTSiyJiIiIiIiISL6SllBKTU1VQimfU2JJRERERERERPIFm81GSkoKKSkpALi5ueXrOUWixJKI=
iIiIiIiIOJndbncklGw2G66urri4aCH7gkCJJRERERERERFxCrvd7hjMrTlKBZMSSyIiIiIiIiJ=
y3VmtVkeVksViUdtbAaXEkoiIiIiIiIhcNxfPUbLb7UooFXBKLImIiIiIiIhInrPb7aSmppKcnK=
w5SjcQfQdFREREREREJM+kJZQSExNJTEwEwN3d/YZLKs2bN4/SpUs7O4zr7sb6LoqIiIiIiIhIn=
hg4cCAWiyXDdvDgwcuekzaYOzExEavVipubG66urtcx6iu73skgi8XC0qVLr9v9rge1womIiIiI=
iIhIlnTu3Jk5c+ak2xcUFJThOJvNRmpqKikpKZdte0tOTsbDwyNP45W8p4olEREREREREaeyA3F=
O2uzZitTT05PSpUun29IqkDZs2EDTpk3x9PSkbNmyjB07ltTUVEfbW8eOHRk1ahTPPvss5cuXp2=
vXrgDs3buXnj17EhgYSKVKlRg8eDCRkZGOe9psNqZOnUqdOnXw9/cnODiYN9980/H8Cy+8QL169=
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
72r+a/JkydTsWJFgoKCGD58OOPHj6dZs2Y5/I6ld2kr3L59++jQoQPe3t7Url2bNWvWYLFYWLp0=
abrzQkNDadeuHT4+PjRo0IDNmzfnSjzXmxJLcs28vc1A71GjzOOxY2HECEhNdWpYIuIEERHw3HN=
QsaL5GBEB5crB1KlmJcnXX4dSpZwXn+YsiYiISH4UHw++vte2+fm5UKKEJ6VL+1K6tC+BgV5Z2t=
JW5c0N48ePZ8SIEezevZv27duTmJhIo0aNWLJkCTt37mTw4MEMGTKEbdu2XfE6M2bM4Oabb2bLl=
i0MHTqUkSNHsm/fviue89JLLzF58mR+/fVX3NzcGDZsmOO5BQsW8Oabb/Laa6+xadMmKlSowKef=
fporr/lSNpuNPn364O3tzZYtW/jkk0944YUXMj32hRde4Omnn2b37t3cdNNN9O3bl9QC+Ie0WuE=
kV7i6wjvvmCXCR4821QjHjsHCheY/ciJyY9u/37S7zZ1rqhcBatWCZ5+FBx4w1UL5QadO5uPmzX=
D+vKmiEhEREZHc8fjjj9OzZ890+0aPHu34fMSIEaxevZolS5bQtGnTy16nU6dOjsTQ008/zfvvv=
09ISAg1atS47DmvvPIKrVu3dpzTq1cvEhMT8fLyYubMmTz00EMMGDAAgOeff541a9YQFxd31dfU=
rl07XFzS1+QkJCRQv379TI9fs2YNYWFhrFy5kipVqmCxWHj99dfp0KFDhmOffvppunbt6oi/Tp0=
6HDx4kJo1a141rvxEiSXJVU8+aSoVHngAfvwR2rQxH/NZC+x1c+wYzJ5tSkwnTgQvL2dHJJK7tm=
41LW/ffvtfGXXLlqZaqVs3M6A7P6lcGWrWNCtZrl0L99zj7IhEREREwMcHYmOzd07aLKXU1FRcX=
V0zJD+yc+/ccvPNN6d7bLVamTp1Kl9//TUnTpwgKSmJpKQkfK5y07p16zo+t1gslCpVijNnzmT5=
nLQZTKdPn6ZixYocOHAgXQUTQJMmTdiwYcNVX9O8efMyJHoGDhx42eP3799P+fLlKXVRmf7lkmg=
XJ6fKlCnjiFmJJSn0evWCdeuge3ezdHjz5rB8OdSu7ezIrg+bDX76CWbOhB9++G/1qf37TctgFu=
bXieRrdrtpJXvzTbj4/8Xdu5uE0q23Oi+2rOjSxSSWVq5UYklERETyB4sFihTJ2rF2u52UlBTs9=
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
7U0mIIlERERERERsZzdbichIYHIyEhSU1PJzMzE5/NpyVYTCA8PJzk5maioKDIzM8nLy8PlcuF2=
u7HZbFaXJwFGS+FERERERESkxXC73XTv3p0uXbqwe/ducnJy8Pv9VpfV6thsNnw+H507dyYlJQW=
Hw0FOTg6lpaVWlyYBRsGSiIiIiIiItChOp5MOHTrQq1cvIiIiyMjI0DygJuJwOGjTpg3dunWjXb=
t2lJWVkZubS2VlpdWlSYDQUjgRERERERFpkaKiooiIiGD79u3s3LkTl8uFz+ezuqxWKTQ0lPbt2=
+Pz+cjIyCAvLw+n04nH48FuV0+KHJi+O0RERERERKTFCg0NJSUlhR49emC328nIyFA3TRNyu92k=
pKTQpUsXXC4XOTk5lJSUWF2WtGDqWBIREREREZEWzWazERcXVzvYOysri8jISNxut9WltUp2u53=
o6Gjcbjc5OTm1O8h5vV5CQ0OtLk9aGHUsiYiIiIiISECIiIigW7dudOnShYqKCrKysqiurra6rF=
YrJCSExMREunXrRkJCAiUlJeTm5lJVVWV1adKCqGNJREREREREAobD4aBdu3a43W5SU1PJzMwkO=
joal8tldWmtVnh4OElJSURFRZGVlUVubi4ulwu3243NZrO6PLGYOpZEREREREQk4Hi9Xnr06EFy=
cjIFBQXk5eXh9/utLqvVstlseL1eOnXqROfOnXE4HOTk5FBaWmp1aWIxBUsiIiIiIiISkEJCQuj=
YsSO9evUiJCSEjIwMKioqrC6rVXM4HMTGxtKtWzfat29PWVkZOTk5+nsPYloKJyIiIiIiIgHLZr=
MRGxtbO9g7IyNDg72bQWhoKO3atcPn85GZmUlOTg4OhwOv14vdrh6WYKJ/bREREREREQl4YWFhd=
O3alW7dulFZWUlWVpaGTDeDyMhIOnXqRNeuXQkPDycnJ4eSkhKry5JmpI4lERERERERaRXsdjuJ=
iYlERkaybds2srKy8Pl8hIeHW11aq2az2YiKisLtdpObm0tGRgY5OTm43W4NVQ8C6lgSERERERG=
RVsXj8dC9e3dSUlIoKSkhNzdXg72bgdPpJD4+nm7duhEfH8/u3bvJzc1V51grp2BJREREREREWh=
2n00lSUhK9evUiLCyMjIwMysvLrS4rKISFhZGcnEzXrl2JiooiPz+foqIihXutlJbCiYiIiIiIS=
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
IiIiIiIiAQLm9/v91tdBJgJ6q+//vp+u4sOpnfv3lx44YXcfffdtddVVVVx8sknM27cOD799FPy=
8/PrdEMNHDiQo48+mqeeeqr2ul69ejFq1CimT59er8ctLCzE5/NRUFCA1+s9pJpFRERERERERFq=
qQ8k8AnrGUnV1NUVFRcTExNS5/r777iMuLo7x48fv8zXl5eWsWrWKYcOG1bl+2LBhfP755wd8rL=
KyMgoLC+ucRERERERERESCWUAHSzNmzKCkpIQLLrig9rrPPvuM5557jtmzZ+/3a7Kzs6mqqiIhI=
aHO9QkJCaSnpx/wsaZPn47P56s9JSUlNc6TEBEREREREREJUAEbLM2fP5+pU6eyYMEC4uPjASgq=
KuLSSy9l9uzZtGnT5qBfb7PZ6lz2+/37XLe3KVOmUFBQUHvatm3b4T8JEREREREREZEA5rS6gIZ=
YsGAB48ePZ+HChZx66qm112/cuJEtW7YwcuTI2uuqq6sBcDqd/PLLLyQlJeFwOPbpTsrMzNyni2=
lvLpcLl8vVyM9ERERERERERCRwBVzH0vz587n88st55ZVXGDFiRJ3bevbsydq1a1mzZk3t6ayzz=
mLIkCGsWbOGpKQkQkNDGTBgAEuXLq3ztUuXLmXw4MHN+VRERERERERERAKapR1LxcXFbNiwofby=
5s2bWbNmDTExMSQnJzNlyhR27NjBCy+8AJhQacyYMTz66KMMGjSotusoPDwcn89HWFgYffr0qfM=
YUVFRAHWunzx5MpdddhnHHHMMxx13HM8++yypqalMmDChiZ+xiIiIiIiIiEjrYWmwtHLlSoYMGV=
J7efLkyQCMHTuWefPmkZaWRmpqau3tzzzzDJWVlUycOJGJEyfWXl9zfH1deOGF5OTkcN9995GWl=
kafPn1YsmQJHTt2PPwnJSIiIiIiIiISJGx+v99vdRGBqLCwEJ/PR0FBAV6v1+pyREREREREREQa=
xaFkHgE3Y0lERERERERERFoGBUsiIiIiIiIiItIgCpZERERERERERKRBFCyJiIiIiIiIiEiDKFg=
SEREREREREZEGUbAkIiIiIiIiIiINomBJREREREREREQaRMGSiIiIiIiIiIg0iNPqAgKV3+8HoL=
Cw0OJKREREREREREQaT03WUZN9HIyCpQYqKioCICkpyeJKREREREREREQaX1FRET6f76DH2Pz1i=
Z9kH9XV1ezcuROPx4PNZrO6nAYpLCwkKSmJbdu24fV6rS5HJOjoZ1DEOvr5E7GOfv5ErKOfP6kv=
v99PUVER7dq1w24/+BQldSw1kN1up0OHDlaX0Si8Xq9eVEQspJ9BEevo50/EOvr5E7GOfv6kPn6=
vU6mGhneLiIiIiIiIiEiDKFgSEREREREREZEGUbAUxFwuF/fccw8ul8vqUkSCkn4GRayjnz8R6+=
jnT8Q6+vmTpqDh3SIiIiIiIiIi0iDqWBIRERERERERkQZRsCQiIiIiIiIiIg2iYElERERERERER=
BpEwZKIiIiIiIiIiDSIgqUg9uSTT5KSkkJYWBgDBgzg008/tbokkVZv6tSp2Gy2OqfExESryxJp=
tZYvX87IkSNp164dNpuNxYsX17nd7/czdepU2rVrR3h4OH/84x/54YcfrClWpJX5vZ+/yy+/fJ/=
fiYMGDbKmWJFWZPr06Rx77LF4PB7i4+MZNWoUv/zyS51j9PtPGpOCpSC1YMECrr/+eu644w5Wr1=
7NiSeeyPDhw0lNTbW6NJFWr3fv3qSlpdWe1q5da3VJIq1WSUkJ/fr14/HHH9/v7Q899BAzZ87k8=
ccf5+uvvyYxMZGhQ4dSVFTUzJWKtD6/9/MHcPrpp9f5nbhkyZJmrFCkdVq2bBkTJ07kyy+/ZOnS=
pVRWVjJs2DBKSkpqj9HvP2lMNr/f77e6CGl+AwcO5Oijj+app56qva5Xr16MGjWK6dOnW1iZSOs=
2depUFi9ezJo1a6wuRSTo2Gw2Xn/9dUaNGgWYT2vbtWvH9ddfz6233gpAWVkZCQkJPPjgg/z1r3=
+1sFqR1uW3P39gOpby8/P36WQSkcaVlZVFfHw8y5Yt46STTtLvP2l06lgKQuXl5axatYphw4bVu=
X7YsGF8/vnnFlUlEjzWr19Pu3btSElJYfTo0WzatMnqkkSC0ubNm0lPT6/z+9DlcnHyySfr96FI=
M/nkk0+Ij4+ne/fu/OUvfyEzM9PqkkRanYKCAgBiYmIA/f6TxqdgKQhlZ2dTVVVFQkJCnesTEhJ=
IT0+3qCqR4DBw4EBeeOEF3nvvPWbPnk16ejqDBw8mJyfH6tJEgk7N7zz9PhSxxvDhw3n55Zf56K=
OPmDFjBl9//TWnnHIKZWVlVpcm0mr4/X4mT57MCSecQJ8+fQD9/pPG57S6ALGOO2xDIgAABpBJR=
EFUzWarc9nv9+9znYg0ruHDh9ee79u3L8cddxxdunTh+eefZ/LkyRZWJhK89PtQxBoXXnhh7fk+=
ffpwzDHH0LFjR95++23OOeccCysTaT2uueYavvvuO/73v//tc5t+/0ljUcdSEGrTpg0Oh2OfNDo=
zM3Of1FpEmlZkZCR9+/Zl/fr1VpciEnRqdmTU70ORlqFt27Z07NhRvxNFGsm1117Lm2++yccff0=
yHDh1qr9fvP2lsCpaCUGhoKAMGDGDp0qV1rl+6dCmDBw+2qCqR4FRWVsZPP/1E27ZtrS5FJOikp=
KSQmJhY5/dheXk5y5Yt0+9DEQvk5OSwbds2/U4UOUx+v59rrrmGRYsW8dFHH5GSklLndv3+k8am=
pXBBavLkyVx22WUcc8wxHHfccTz77LOkpqYyYcIEq0sTadVuuukmRo4cSXJyMpmZmTzwwAMUFhY=
yduxYq0sTaZWKi4vZsGFD7eXNmzezZs0aYmJiSE5O5vrrr2fatGl069aNbt26MW3aNCIiIrj44o=
strFqkdTjYz19MTAxTp07l3HPPpW3btmzZsoXbb7+dNm3acPbZZ1tYtUjgmzhxIq+88gpvvPEGH=
o+ntjPJ5/MRHh6OzWbT7z9pVDa/3++3ugixxpNPPslDDz1EWloaffr04V//+hcnnXSS1WWJtGqj=
R49m+fLlZGdnExcXx6BBg7j//vs54ogjrC5NpFX65JNPGDJkyD7Xjx07lnnz5uH3+7n33nt55pl=
nyMvLY+DAgTzxxBO1A05FpOEO9vP31FNPMWrUKFavXk1+fj5t27ZlyJAh3H///SQlJVlQrUjrca=
A5SXPnzuXyyy8H0O8/aVQKlkREREREREREpEE0Y0lERERERERERBpEwZKIiIiIiIiIiDSIgiURE=
REREREREWkQBUsiIiIiIiIiItIgCpZERERERERERKRBFCyJiIiIiIiIiEiDKFgSEREREREREZEG=
UbAkIiIiIiIiIiINomBJREREREREREQaRMGSiIiIiAUuv/xybDYbNpuNkJAQEhISGDp0KHPmzKG=
6utrq8kRERETqRcGSiIiIiEVOP/100tLS2LJlC++88w5Dhgxh0qRJnHnmmVRWVlpdnoiIiMjvUr=
AkIiIiYhGXy0ViYiLt27fn6KOP5vbbb+eNN97gnXfeYd68eQDMnDmTvn37EhkZSVJSEn/7298oL=
i4GoKSkBK/Xy2uvvVbnft966y0iIyMpKipq7qckIiIiQUbBkoiIiEgLcsopp9CvXz8WLVoEgN1u=
Z9asWXz//fc8//zzfPTRR9xyyy0AREZGMnr0aObOnVvnPubOnct5552Hx+Np9vpFREQkuNj8fr/=
f6iJEREREgs3ll19Ofn4+ixcv3ue20aNH89133/Hjjz/uc9vChQu5+uqryc7OBuCrr75i8ODBpK=
am0q5dO7Kzs2nXrh1Lly7l5JNPbuqnISIiIkFOHUsiIiIiLYzf78dmswHw8ccfM3ToUNq3b4/H4=
2HMmDHk5ORQUlICwB/+8Ad69+7NCy+8AMCLL75IcnIyJ510kmX1i4iISPBQsCQiIiLSwvz000+k=
pKSwdetWzjjjDPr06cN//vMfVq1axRNPPAFARUVF7fFXXnll7XK4uXPnMm7cuNpgSkRERKQpKVg=
SERERaUE++ugj1q5dy7nnnsvKlSuprKxkxowZDBo0iO7du7Nz5859vubSSy8lNTWVWbNm8cMPPz=
B27FgLKhcREZFg5LS6ABEREZFgVVZWRnp6OlVVVWRkZPDuu+8yffp0zjzzTMaMGcPatWuprKzks=
cceY+TIkXz22Wc8/fTT+9xPdHQ055xzDjfffDPDhg2jQ4cOFjwbERERCUbqWBIRERGxyLvvvkvb=
tm3p1KkTp59+Oh9//DGzZs3ijTfewOFwcNRRRzFz5kwefPBB+vTpw8svv8z06dP3e1/jx4+nvLy=
cK664opmfhYiIiAQz7QonIiIi0gq8/PLLTJo0iZ07dxIaGmp1OSIiIhIktBROREREJIDt2rWLzZ=
s3M336dP76178qVBIREZFmpaVwIiIiIgHsoYce4qijjiIhIYEpU6ZYXY6IiIgEGS2FExERERERE=
RGRBlHHkoiIiIiIiIiINIiCJRERERERERERaRAFSyIiIiIiIiIi0iAKlkREREREREREpEEULImI=
iIiIiIiISIMoWBIRERERERERkQZRsCQiIiIiIiIiIg2iYElERERERERERBrk/wGF8CbMqLmmbQA=
AAABJRU5ErkJggg=3D=3D"></div></div></div><div class=3D"btn btn-default outp=
ut_collapsed" title=3D"click to expand output" style=3D"display: none;">. .=
 .</div></div></div><div class=3D"cell code_cell rendered unselected" tabin=
dex=3D"2"><div class=3D"input"><div class=3D"prompt_container"><div class=
=3D"prompt input_prompt"><bdi>In</bdi>&nbsp;[20]:</div><div class=3D"run_th=
is_cell" title=3D"Run this cell"><i class=3D"fa-step-forward fa"></i></div>=
</div><div class=3D"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"c=
elltoolbar"></div></div><div class=3D"input_area" aria-label=3D"Edit code h=
ere"><div class=3D"CodeMirror cm-s-ipython"><div style=3D"overflow: hidden;=
 position: relative; width: 3px; height: 0px; top: 22.6px; left: 612px;"><t=
extarea autocorrect=3D"off" autocapitalize=3D"off" spellcheck=3D"false" tab=
index=3D"0" style=3D"position: absolute; bottom: -1em; padding: 0px; width:=
 1000px; height: 1em; outline: none;"></textarea></div><div class=3D"CodeMi=
rror-vscrollbar" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"min-=
width: 1px; height: 0px;"></div></div><div class=3D"CodeMirror-hscrollbar" =
tabindex=3D"-1" cm-not-content=3D"true" style=3D"display: block; right: 0px=
; left: 34px;"><div style=3D"height: 100%; min-height: 1px; width: 653.588p=
x;"></div></div><div class=3D"CodeMirror-scrollbar-filler" cm-not-content=
=3D"true"></div><div class=3D"CodeMirror-gutter-filler" cm-not-content=3D"t=
rue"></div><div class=3D"CodeMirror-scroll" tabindex=3D"-1"><div class=3D"C=
odeMirror-sizer" style=3D"margin-left: 34px; min-width: 653.588px; margin-b=
ottom: -17px; border-right-width: 33px; min-height: 45px; padding-right: 0p=
x; padding-bottom: 17px;"><div style=3D"position: relative; top: 0px;"><div=
 class=3D"CodeMirror-lines" role=3D"presentation"><div role=3D"presentation=
" style=3D"position: relative; outline: none;"><div class=3D"CodeMirror-mea=
sure"><pre class=3D"CodeMirror-line-like">x</pre></div><div class=3D"CodeMi=
rror-measure"></div><div style=3D"position: relative; z-index: 1;"><div cla=
ss=3D"CodeMirror-selected" style=3D"position: absolute; left: 4px; top: 0px=
; width: 645.588px; height: 17px;"></div><div class=3D"CodeMirror-selected"=
 style=3D"position: absolute; left: 4px; top: 17px; width: 646.588px; heigh=
t: 17px;"></div></div><div class=3D"CodeMirror-cursors" style=3D""></div><d=
iv class=3D"CodeMirror-code" role=3D"presentation"><div style=3D"position: =
relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: 30.8px;"=
><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: =
0px; width: 21px;">1</div></div><pre class=3D" CodeMirror-line " role=3D"pr=
esentation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><sp=
an class=3D"cm-variable">w</span><span class=3D"cm-operator">=3D</span><spa=
n class=3D"cm-variable">pred</span>()</span></pre></div><div style=3D"posit=
ion: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: 30.=
8px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"l=
eft: 0px; width: 21px;">2</div></div><pre class=3D" CodeMirror-line " role=
=3D"presentation"><span role=3D"presentation" style=3D"padding-right: 0.1px=
;"><span class=3D"cm-variable">eurusdData</span><span class=3D"cm-operator"=
>=3D</span><span class=3D"cm-variable">w</span>.<span class=3D"cm-property"=
>getData</span>(<span class=3D"cm-string">'https://www.investing.com/curren=
cies/eur-usd-historical-data'</span>)</span></pre></div></div></div></div><=
/div></div><div style=3D"position: absolute; height: 33px; width: 1px; bord=
er-bottom: 17px solid transparent; top: 45px;"></div><div class=3D"CodeMirr=
or-gutters" style=3D"height: 95px; left: 64.8px;"><div class=3D"CodeMirror-=
gutter CodeMirror-linenumbers" style=3D"width: 33px;"></div></div></div></d=
iv></div></div></div><div class=3D"output_wrapper"><div class=3D"out_prompt=
_overlay prompt" title=3D"click to scroll output; double click to hide"></d=
iv><div class=3D"output"></div><div class=3D"btn btn-default output_collaps=
ed" title=3D"click to expand output" style=3D"display: none;">. . .</div></=
div></div><div class=3D"cell code_cell rendered unselected" tabindex=3D"2">=
<div class=3D"input"><div class=3D"prompt_container"><div class=3D"prompt i=
nput_prompt"><bdi>In</bdi>&nbsp;[21]:</div><div class=3D"run_this_cell" tit=
le=3D"Run this cell"><i class=3D"fa-step-forward fa"></i></div></div><div c=
lass=3D"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"celltoolbar">=
</div></div><div class=3D"input_area" aria-label=3D"Edit code here"><div cl=
ass=3D"CodeMirror cm-s-ipython"><div style=3D"overflow: hidden; position: r=
elative; width: 3px; height: 0px; top: 5.60001px; left: 168.863px;"><textar=
ea autocorrect=3D"off" autocapitalize=3D"off" spellcheck=3D"false" tabindex=
=3D"0" style=3D"position: absolute; bottom: -1em; padding: 0px; width: 1000=
px; height: 1em; outline: none;"></textarea></div><div class=3D"CodeMirror-=
vscrollbar" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"min-width=
: 1px; height: 0px;"></div></div><div class=3D"CodeMirror-hscrollbar" tabin=
dex=3D"-1" cm-not-content=3D"true"><div style=3D"height: 100%; min-height: =
1px; width: 0px;"></div></div><div class=3D"CodeMirror-scrollbar-filler" cm=
-not-content=3D"true"></div><div class=3D"CodeMirror-gutter-filler" cm-not-=
content=3D"true"></div><div class=3D"CodeMirror-scroll" tabindex=3D"-1"><di=
v class=3D"CodeMirror-sizer" style=3D"margin-left: 34px; min-width: 137.863=
px; margin-bottom: -17px; border-right-width: 33px; min-height: 28px; paddi=
ng-right: 0px; padding-bottom: 0px;"><div style=3D"position: relative; top:=
 0px;"><div class=3D"CodeMirror-lines" role=3D"presentation"><div role=3D"p=
resentation" style=3D"position: relative; outline: none;"><div class=3D"Cod=
eMirror-measure"><pre class=3D"CodeMirror-line-like">x</pre></div><div clas=
s=3D"CodeMirror-measure"></div><div style=3D"position: relative; z-index: 1=
;"><div class=3D"CodeMirror-selected" style=3D"position: absolute; left: 4p=
x; top: 0px; width: 130.863px; height: 17px;"></div></div><div class=3D"Cod=
eMirror-cursors" style=3D""></div><div class=3D"CodeMirror-code" role=3D"pr=
esentation"><div style=3D"position: relative;"><div class=3D"CodeMirror-gut=
ter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber Cod=
eMirror-gutter-elt" style=3D"left: 0px; width: 21px;">1</div></div><pre cla=
ss=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presentation" =
style=3D"padding-right: 0.1px;"><span class=3D"cm-builtin">print</span>(<sp=
an class=3D"cm-variable">eurusdData</span>)</span></pre></div></div></div><=
/div></div></div><div style=3D"position: absolute; height: 33px; width: 1px=
; border-bottom: 0px solid transparent; top: 28px;"></div><div class=3D"Cod=
eMirror-gutters" style=3D"height: 61px; left: 0px;"><div class=3D"CodeMirro=
r-gutter CodeMirror-linenumbers" style=3D"width: 33px;"></div></div></div><=
/div></div></div></div><div class=3D"output_wrapper"><div class=3D"out_prom=
pt_overlay prompt" title=3D"click to scroll output; double click to hide"><=
/div><div class=3D"output"><div class=3D"output_area"><div class=3D"run_thi=
s_cell"></div><div class=3D"prompt"></div><div class=3D"output_subarea outp=
ut_text output_stream output_stdout" dir=3D"auto"><pre>          Date   Pri=
ce    Open    High     Low
0   01-26-2024  1.0852  1.0843  1.0885  1.0812
1   01-29-2024  1.0833  1.0849  1.0850  1.0796
2   01-30-2024  1.0840  1.0833  1.0857  1.0811
3   01-31-2024  1.0816  1.0844  1.0889  1.0795
4   02-01-2024  1.0872  1.0814  1.0876  1.0779
5   02-02-2024  1.0784  1.0873  1.0898  1.0780
6   02-05-2024  1.0741  1.0784  1.0787  1.0723
7   02-06-2024  1.0754  1.0743  1.0763  1.0723
8   02-07-2024  1.0771  1.0755  1.0784  1.0753
9   02-08-2024  1.0776  1.0772  1.0790  1.0741
10  02-09-2024  1.0782  1.0779  1.0796  1.0761
11  02-12-2024  1.0771  1.0781  1.0806  1.0755
12  02-13-2024  1.0709  1.0772  1.0796  1.0700
13  02-14-2024  1.0725  1.0710  1.0735  1.0695
14  02-15-2024  1.0771  1.0727  1.0785  1.0725
15  02-16-2024  1.0774  1.0770  1.0788  1.0732
16  02-19-2024  1.0777  1.0776  1.0790  1.0761
17  02-20-2024  1.0803  1.0779  1.0840  1.0761
18  02-21-2024  1.0817  1.0807  1.0825  1.0790
19  02-22-2024  1.0823  1.0816  1.0889  1.0802
20  02-23-2024  1.0818  1.0824  1.0841  1.0812
21  02-25-2024  1.0819  1.0826  1.0833  1.0818
22  02-26-2024  1.0852  1.0819  1.0860  1.0812
</pre></div></div></div><div class=3D"btn btn-default output_collapsed" tit=
le=3D"click to expand output" style=3D"display: none;">. . .</div></div></d=
iv><div class=3D"cell code_cell rendered unselected" tabindex=3D"2"><div cl=
ass=3D"input"><div class=3D"prompt_container"><div class=3D"prompt input_pr=
ompt"><bdi>In</bdi>&nbsp;[22]:</div><div class=3D"run_this_cell" title=3D"R=
un this cell"><i class=3D"fa-step-forward fa"></i></div></div><div class=3D=
"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"celltoolbar"></div><=
/div><div class=3D"input_area" aria-label=3D"Edit code here"><div class=3D"=
CodeMirror cm-s-ipython"><div style=3D"overflow: hidden; position: relative=
; width: 3px; height: 0px; top: 22.6px; left: 245.844px;"><textarea autocor=
rect=3D"off" autocapitalize=3D"off" spellcheck=3D"false" tabindex=3D"0" sty=
le=3D"position: absolute; bottom: -1em; padding: 0px; width: 1000px; height=
: 1em; outline: none;"></textarea></div><div class=3D"CodeMirror-vscrollbar=
" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"min-width: 1px; hei=
ght: 0px;"></div></div><div class=3D"CodeMirror-hscrollbar" tabindex=3D"-1"=
 cm-not-content=3D"true"><div style=3D"height: 100%; min-height: 1px; width=
: 0px;"></div></div><div class=3D"CodeMirror-scrollbar-filler" cm-not-conte=
nt=3D"true"></div><div class=3D"CodeMirror-gutter-filler" cm-not-content=3D=
"true"></div><div class=3D"CodeMirror-scroll" tabindex=3D"-1"><div class=3D=
"CodeMirror-sizer" style=3D"margin-left: 34px; min-width: 261.025px; margin=
-bottom: -17px; border-right-width: 33px; min-height: 45px; padding-right: =
0px; padding-bottom: 0px;"><div style=3D"position: relative; top: 0px;"><di=
v class=3D"CodeMirror-lines" role=3D"presentation"><div role=3D"presentatio=
n" style=3D"position: relative; outline: none;"><div class=3D"CodeMirror-me=
asure"><pre class=3D"CodeMirror-line-like">x</pre></div><div class=3D"CodeM=
irror-measure"></div><div style=3D"position: relative; z-index: 1;"><div cl=
ass=3D"CodeMirror-selected" style=3D"position: absolute; left: 4px; top: 0p=
x; width: 580px; height: 17px;"></div><div class=3D"CodeMirror-selected" st=
yle=3D"position: absolute; left: 4px; top: 17px; width: 207.844px; height: =
17px;"></div></div><div class=3D"CodeMirror-cursors" style=3D""></div><div =
class=3D"CodeMirror-code" role=3D"presentation"><div style=3D"position: rel=
ative;"><div class=3D"CodeMirror-gutter-wrapper" style=3D"left: -34px;"><di=
v class=3D"CodeMirror-linenumber CodeMirror-gutter-elt" style=3D"left: 0px;=
 width: 21px;">1</div></div><pre class=3D" CodeMirror-line " role=3D"presen=
tation"><span role=3D"presentation" style=3D"padding-right: 0.1px;"><span c=
lass=3D"cm-variable">warnings</span>.<span class=3D"cm-property">filterwarn=
ings</span>(<span class=3D"cm-string">"ignore"</span>)</span></pre></div><d=
iv style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" s=
tyle=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter=
-elt" style=3D"left: 0px; width: 21px;">2</div></div><pre class=3D" CodeMir=
ror-line " role=3D"presentation"><span role=3D"presentation" style=3D"paddi=
ng-right: 0.1px;"><span class=3D"cm-variable">forcast</span><span class=3D"=
cm-operator">=3D</span><span class=3D"cm-variable">w</span>.<span class=3D"=
cm-property">estim</span>(<span class=3D"cm-variable">eurusdData</span>)</s=
pan></pre></div></div></div></div></div></div><div style=3D"position: absol=
ute; height: 33px; width: 1px; border-bottom: 0px solid transparent; top: 4=
5px;"></div><div class=3D"CodeMirror-gutters" style=3D"height: 78px; left: =
0px;"><div class=3D"CodeMirror-gutter CodeMirror-linenumbers" style=3D"widt=
h: 33px;"></div></div></div></div></div></div></div><div class=3D"output_wr=
apper"><div class=3D"out_prompt_overlay prompt" title=3D"click to scroll ou=
tput; double click to hide"></div><div class=3D"output"><div class=3D"outpu=
t_area"><div class=3D"run_this_cell"></div><div class=3D"prompt"></div><div=
 class=3D"output_subarea output_png" dir=3D"auto"><img src=3D"data:image/pn=
g;base64,iVBORw0KGgoAAAANSUhEUgAABJYAAAJuCAYAAADihog9AAAAOXRFWHRTb2Z0d2FyZQ=
BNYXRwbG90bGliIHZlcnNpb24zLjcuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8pXeV/AAAAC=
XBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOzdd3hU1drG4d9k0itpEOnFCChN4YAoXYqgIogN=
RZqCYkFQVBCwACIoqFgOqAekiFgRUWwgVakREAudAEkIhIQU0pOZ/f2xv4yEUJKQMCnPfa65smf=
PLu9O0GMe1nqXxTAMAxERERERERERkSJycXYBIiIiIiIiIiJSPilYEhERERERERGRYlGwJCIiIi=
IiIiIixaJgSUREREREREREikXBkoiIiIiIiIiIFIuCJRERERERERERKRYFSyIiIiIiIiIiUiwKl=
kREREREREREpFgULImIiIiIiIiISLEoWBIREZFCefvtt7FYLDRp0uS8x1gslnwvf39/brjhBpYs=
WVLg2Pnz52OxWIiIiHDse+mll7BYLLi4uHDo0KEC56SlpeHv74/FYmHw4MHnrOHPP//EYrHg5uZ=
GbGxsoZ+vJO5dHIcPH8ZisTB//vwin7t27VosFgtr164t1HHnexXn3oU1ePBg6tatW2rXBzh27B=
gvvfQSO3fuLPBZ3s9VRERESoeCJRERESmUefPmAfD333+zZcuW8x535513smnTJjZu3MicOXNIS=
Unhvvvu45NPPin0vXx9ffnoo48K7P/iiy/IycnBzc3tvOf+73//AyA3N5eFCxcW+p4lce+yburU=
qWzatKnA65ZbbnF2aZfk2LFjvPzyy+cMlh566CE2bdp0+YsSERGpJBQsiYiIyEVFRETwxx9/OAK=
IuXPnnvfYatWqcf3119O2bVvuu+8+VqxYAcD7779f6Pvdc889LFiwALvdnm//3Llz6du3L+7u7u=
c8Lysri8WLF9O8eXNq1KjhCMOKorj3Lg/Cw8O5/vrrC7xCQ0OdXVqpqVmzJtdff72zyxAREamwF=
CyJiIjIReUFSdOmTeOGG27g008/JT09vVDn1qlTh9DQUE6cOFHo+w0dOpSoqChWrlzp2Ldv3z5+=
/fVXhg4det7zli1bRkJCAg899BCDBg1ynFMUxbn30aNHGTBgAFWrVsXDw4PGjRszc+bMAuHUsWP=
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
m2x8fH0+VKlWK8FT/yvvzERsbS82aNfN9duzYMcf3X0RERApHI5ZERETknGw2GwsWLKBBgwasWb=
OmwOvpp58mNjaWH3744YLXad++PQMHDmTFihVs2rSpSDW0bduWoUOH0rdvX/r27Xve4+bOnYuLi=
wvLli0rUOeiRYuAc4+uKol733TTTfzzzz9s37493/6FCxdisVjo3LkzAJ07d+b06dMsX74833Gf=
fPJJvvcNGzYkPDycP/7445yji1q1aoWfn1+RnqWohgwZwpYtW/j111/59ttvGTRoUL7wMG+VNQ8=
PD8c+wzD48MMPL3rtatWq4enpya5du/Lt/+abbwoca7FY8t0DYMWKFcTExOTbl3dMYUYRdenSBa=
BA8+1t27axe/fuCzaHFxERkYI0YklERETO6YcffuDYsWNMnz6dTp06Ffi8SZMmvPvuu8ydO5dbb=
731gteaPHkyn332GRMnTmTVqlVFquNi09gSEhL45ptv6NGjB7fffvs5j3nzzTdZuHAhr776ar5p=
X5d6b4DRo0ezcOFCbrnlFiZNmkSdOnVYsWIF//3vfxkxYoRjNbyBAwfy5ptvMnDgQF555RXCw8P=
5/vvv+emnnwpc8/3336dnz5706NGDwYMHU6NGDU6dOsXu3bvZvn17oVfkO9v+/fvZvHlzgf01a9=
bMN3qnf//+PPXUU/Tv35+srKwC/Yi6deuGu7s7/fv359lnnyUzM5PZs2eTmJh40RosFgsDBgxg3=
rx5NGjQgObNm7N169YCARvArbfeyvz582nUqBHNmjXj999/5/XXXy8w0qhBgwZ4eXmxePFiGjdu=
jK+vL9WrV3dMRzxTw4YNGT58OO+88w4uLi707NmTw4cPM3HiRGrVqsXo0aMv+gwiIiLyL41YEhE=
RkXOaO3cu7u7u+XrrnCkkJIS+ffvy3XffOfoCnU+tWrV44okn+OWXX1i/fn2J1vnxxx+TlZV1wW=
Xuhw8fzsmTJ/n2229L9N5gTv3buHEjXbp0Ydy4cdx666389NNPvPbaa7zzzjuO47y9vVm9ejVdu=
3Zl7Nix3HnnnURHRzt6GZ2pc+fObN26lSpVqjBq1Ci6du3KiBEjWLVqFV27di12rc8//zxt27Yt=
8JozZ06+4wICAujbty/R0dHceOONjnAsT6NGjfjqq69ITEzkjjvu4IknnqBFixa8/fbbhapj5sy=
ZDBgwgNdee43bb7+dTZs2nXOa5KxZsxgwYACvvvoqt912G8uXL2fp0qU0aNAg33He3t7MmzePhI=
QEunfvzn/+8x8++OCD895/9uzZTJs2je+//55bb72V8ePH0717dzZu3HjOqZQiIiJyfhbDMAxnF=
yEiIiIiIiIiIuWPRiyJiIiIiIiIiEixKFgSEREREREREZFiUbAkIiIiIiIiIiLFomBJRERERERE=
RESKRcGSiIiIiIiIiIgUi4IlEREREREREREpFldnF1Be2e12jh07hp+fHxaLxdnliIiIiIiIiIi=
UCMMwOH36NNWrV8fF5cJjkhQsFdOxY8eoVauWs8sQERERERERESkVUVFR1KxZ84LHKFgqJj8/P8=
D8Jvv7+zu5GhERERERERGRkpGSkkKtWrUc2ceFKFgqprzpb/7+/gqWRERERERERKTCKUzrHzXvF=
hERERERERGRYlGwJCIiIiIiIiIixaJgSUREREREREREikU9lkREREREREScwGazkZOT4+wypBKy=
Wq24uroWqofSxShYEhEREREREbnMUlNTiY6OxjAMZ5cilZS3tzdXXHEF7u7ul3QdBUsiIiIiIiI=
il5HNZiM6Ohpvb29CQ0NLZNSISGEZhkF2djYnT54kMjKS8PBwXFyK3ylJwZKIiIiIiIjIZZSTk4=
NhGISGhuLl5eXscqQS8vLyws3NjSNHjpCdnY2np2exr6Xm3SIiIiIiIiJOoJFK4kyXMkop33VK5=
CoiIiIiIiIiIlLpKFgSEREREREREZFiUbAkIiIiIiIiIk7RqVMnRo0aVejjDx8+jMViYefOnaVW=
kxSNgiURERERERERuSCLxXLB1+DBg4t13aVLlzJ58uRCH1+rVi1iY2Np0qRJse5XWAqwCk+rwom=
IiIiIiIjIBcXGxjq2P/vsM1544QX27t3r2Hf26nY5OTm4ubld9LpBQUFFqsNqtRIWFlakc6R0ac=
SSiIiIiIiIiDMZBqSlOedlGIUqMSwszPEKCAjAYrE43mdmZlKlShU+//xzOnXqhKenJx9//DEJC=
Qn079+fmjVr4u3tTdOmTVmyZEm+6549Fa5u3bpMnTqVoUOH4ufnR+3atfnggw8cn589kmjt2rVY=
LBZ++eUXWrVqhbe3NzfccEO+0AtgypQpVK1aFT8/Px566CHGjh1LixYtivXjAsjKymLkyJFUrVo=
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
/nnnmGcaNG0fbtm05fPgwAwYMwMPDo8TvZbVa+fTTT0lLS6N169Y89NBDTJgwAaDChpAWo7ATCy=
WflJQUAgICSE5Oxt/f39nliIiIiIiISCnIzMwkOjqa48eP4+7uTkBAwCUHSjabjZycHOrUqVMq4=
YZc3C233EK1atWYN29eiV/bZrMB4O3tjcVi4bfffqNdu3YcOHCgQL8mZ8obgVevXr0CoVdRMg81=
7xYRERERERE5S94opaioKNLS0ggMDMTd3d3ZZUkxpKen8+GHH9KtWzesViuff/45q1evZsWKFaV=
yv+XLl+Pr60uTJk04ePAgTz75JDfeeGOZCpVKkoIlERERERERkTNkZGQQExNDbGwsHh4eVK1aVd=
PeyjGLxcJPP/3E9OnTycrK4qqrrmLJkiV06dKlVO6XmprKxIkTiY6OJiQkhK5duzJz5sxSuVdZo=
KlwxaSpcCIiIiIiIhWL3W7PN0opKCioVEYpaSpcxXb2VLiySlPhREREREREREpIeno60dHRnDhx=
Ak9PT8LCwpxdkki5oGBJREREREREKi273c7JkyeJiooiIyODoKAg3NzcnF2WSLmhYElEREREREQ=
qpfT0dKKiooiLi8PLy4tq1ao5uySRckfBkoiIiIiIiFQqGqUkUnIULImIiIiIiEilkZaWRlRUFC=
dPnsTb21ujlEQukYIlERERERERqfBsNptjlFJmZibBwcG4uupXYpFL5eLsAkRERERERERKU2pqK=
vv372ffvn1YrVaqVaumUKkC8vLyYvny5Zd8nUWLFhV5VcBhw4Zx1113XfK9yyMFSyIiIiIiIlIh=
2Ww2YmNj+eeffzh58iQhISH4+vo6u6xyb9OmTfj4+NC7d+8in9uwYUPeeeedUqjq4s4X/qxfvx4=
vLy+SkpIAuPPOO9m1a9dlrq78UrAkIiIiIiIiFc7p06fZu3cvBw4cwNXVVaOUStDChQsZMWIEGz=
du5OjRo84up8R5eXlRtWpVZ5dRbihYEhERERERkQrDZrMRExPDP//8w6lTpwgODi7zo5QMA9LSn=
PMyjKLVmpaWxldffcXw4cPp2bMnH3/8cYFjvvvuO2688UaqVKlCzZo1ueeeewDo3r07R48e5dln=
n8XLywsvLy8ApkyZQps2bfJd45133qFhw4aO9xEREdxyyy3UrFmTatWq0a1bN3bs2FHE73ThnGs=
q3LRp06hduzahoaGMGDGCCRMmFKgZ4M0336RBgwbUrl2bxx57jJycnFKpsSxRXCsiIiIiIiIVwu=
nTp4mKiiI+Ph5fX18CAwOdXVKhpKdDSIinU+4dH5+Jj0/hj//yyy8JDw/nqquuon///jz11FOMG=
zcOi8UCwA8//MC9997Lc889x9y5c8nOzubHH38E4NNPP6V169Y8+OCDDBkypEh1pqamMmDAAGbO=
nAnArFmz6Nu3L3/++Sd+fn5FulZRLVmyhOnTpzNr1izatm3LF198waxZs6hbt26+49avX88VV1z=
B999/z6FDhxg0aBDXXnstw4YNK9X6nE3BkoiIiIiIiJRrubm5nDhxgujoaHJzcwkNDcVqtTq7rA=
pp/vz59O/fHzBHIKWlpbFmzRq6dOkCwPTp07nrrruYOHGi45xmzZoBEBQUhNVqxdfXt8jNsTt16=
pTv/bvvvssVV1zBhg0b6NWrV6Gv88MPPxASEpJvn81mu+A5s2fPZtCgQQwcOBCA559/nlWrVpGW=
lpbvuCpVqvDmm28CZi+pW265hV9++UXBkoiIiIiIiEhZlZKSQlRUFAkJCfj5+ZWbUUpn8vY2Rw4=
5696FtW/fPiIiIvj0008BcHV1pV+/fixYsMARLO3atYuhQ4eWeJ1xcXFMnjyZtWvXEhcXh81mIz=
09naioqCJdp2PHjrz99tv59m3duvWCNe/fv5+HH344375WrVqxbt26fPuuvvpqrFarI6gKCwvjr=
7/+KlJ95ZGCJRERERERESl3cnNzOX78ODExMeV+lJLFQpGmoznL/Pnzyc3NpUGDBo59hmHg5uZG=
YmIigYGBjr5JReHi4oJxVrOns3sTDR8+nJMnT/L6669Tu3ZtPDw86NSpE9nZ2UW6l7e3d776AWJ=
iYi56Xt5Uvzxn1wsUaA5vsViw2+1Fqq88UvNuERERERERKVeSk5PZu3cvhw4dwsPDo1yHSuVFbm=
4un3zyCdOmTWPLli2O19atW6ldu7ZjFFOTJk1Ys2bNea/j7u5eYOpZSEgIJ06cyBfW7Nq1K98xv=
/32G4899hg333wzV199Ne7u7sTHx5fgE55feHg427Zty7dv+/btl+Xe5YGCJRERERERESkXcnJy=
iIqKYvfu3SQnJ1O1alW8izKXS4rt+++/JzExkcGDB3PNNdfke/Xt25cFCxYAMH78eD7//HMmT57=
Mnj17+OuvvxwNtwHq1KnDb7/9RkxMjCMY6tChAydPnmTmzJkcOnSIOXPm8PPPP+e7f4MGDfjkk0=
/Ys2cPW7duZciQIcUaHVUcI0aMYMGCBXz88cccOHCAadOm8ddffxUYxVRZKVgSERERERGRMi8pK=
ckxSsnT05OQkBBcXPQr7eWS10cpICCgwGd9+vThjz/+YMeOHXTo0IHFixezYsUK2rRpQ8+ePfON=
9pk4cSJHjhzhmmuuoVatWgA0atSIWbNm8f7779O6dWsiIiIYNWpUvnvMmTOHxMRErr/+eh588EE=
effRRQkNDS/WZ8/Tv359nnnmGcePG0bZtWw4fPsyAAQPw8PC4LPcv6yzGuSYGykWlpKQQEBBAcn=
Iy/v7+zi5HRERERESkQsrJyeHYsWMcO3YMwzAICgoq94GSzWYjJyeHOnXqKJwop2655RaqVavGv=
HnzCnyWN9XP29u7TI9qyszMJDIyknr16uHp6Znvs6JkHmreLSIiIiIiImVSYmIiUVFRJCUlERAQ=
cNmmPomcKT09nQ8//JBu3bphtVr5/PPPWb16NStWrHB2aWWCgiUREREREREpU7Kzs4mNjSUmJga=
LxULVqlXL/SglKb8sFgs//fQT06dPJysri6uuuoolS5bQpUsXZ5dWJihYEhERERERkTIjMTGRo0=
ePkpSURGBgYIEpOiKXm5eXF99//72zyyizFCyJiIiIiIiI02VnZ3Ps2DFiYmKwWq2EhYWV6f40I=
mJSsCQiIiIiIiJOl5CQwOHDhwkODlZDa5FyRJNURURERERExOnsdjtWq1Whkkg5o2BJRERERERE=
RESKxanB0vr167ntttuoXr06FouFZcuWXfScdevW0bJlSzw9Palfvz5z5szJ93lOTg6TJk2iQYM=
GeHp60rx5c3788ccC1/nvf/9LvXr18PT0pGXLlmzYsKGkHktEREREREREpFJwarCUlpZG8+bNef=
fddwt1fGRkJL169aJ9+/bs2LGD559/npEjR/LVV185jpkwYQLvv/8+77zzDv/88w+PPPIIffv2Z=
ceOHY5jPvvsM0aNGsX48ePZsWMH7du3p2fPnhw9erTEn1FEREREREREpKKyGIZhOLsIAIvFwtdf=
f02fPn3Oe8xzzz3H8uXL2b17t2PfI488wh9//MGmTZsAqF69OuPHj+exxx5zHNOnTx98fX35+OO=
PAWjTpg3XXXcds2fPdhzTuHFj+vTpw6uvvlqoelNSUggICCA5ORl/f/+iPKqIiIiIiIicJSYmhk=
OHDlGtWjVnl1LqbDYbOTk51KlTRz2lKpBFixbxzDPPEBMTA4C3t3exVzbs1KkTLVq04K233ir0O=
YXJVc6UmZlJZGSkYzbXmYqSeZSrHkubNm2ie/fu+fb16NGDiIgIcnJyAMjKyirwDfHy8uLXX38F=
zCUsf//99wLX6d69Oxs3bjzvvbOyskhJScn3EhEREREREakshg0bhpeXV4HXwYMHnV1asS1atIi=
wsLDLdr/ztQEaPHhwvkBo6dKlTJ48+bLVdSnKVbB0/PjxAul1tWrVyM3NJT4+HjCDpjfeeIP9+/=
djt9tZuXIl33zzDbGxsQDEx8djs9nOeZ3jx4+f996vvvoqAQEBjletWrVK+OlEREREREREyrbu3=
bsTGRmZ71W3bt1iXSs7O7tki6tAgoKC8PPzc3YZhVKugiWgwDCyvJl8eftnzZpFeHg4jRo1wt3d=
nccff5whQ4ZgtVovep0LDVEbN24cycnJjldUVFRJPI6IiIiIiIhUcoZhkJad5pRXUbvjuLu7ExY=
Wlu+V9/v2hg0baNeuHQEBAdSrV48JEyaQm5vrOLd79+6MGjWKZ599lpo1a3LLLbcAsHv3bvr06U=
NISAh16tRh6NChjsEjAHa7nRkzZnDNNdcQEBBAeHg406dPd3w+fvx4mjZtSlBQEI0bN+bll192z=
GoC2LVrFz169CA0NJSqVatyww038Pvvv7N+/XqGDx9OcnKyY/TVlClTADP0ev7556lfvz7BwcG0=
b9+e9evX5/teLFq0iPDwcIKCgrj77rtJSEgo0vfyQjp16sSoUaMc72NjY7nlllvw8vKiXr16fPL=
JJ9StW7fAVLn4+Hj69u2Lt7c34eHhLF++vMRqOh/XUr9DCQoLCyswqiguLg5XV1eCg4MBCA0NZd=
myZWRmZpKQkED16tUZO3Ys9erVAyAkJASr1XrO61xoLq+Hh4fmvopIiTl6FN56CwYMgOuuc3Y1I=
iIiIuJM6TnphLwZ4pR7x4+Ox8fd55KvExMTQ58+fXjggQeYO3cue/fu5bHHHsPT05MJEyY4jlu8=
eDHDhg1j9erVGIZBbGws3bt3Z8iQIUyfPp2MjAwmTJjAgAEDHCu8T5w4kY8++ojXXnuNG264gdj=
YWPbt2+e4pp+fHx988AHVq1fnr7/+4rHHHsPX15enn34agCFDhtC8eXPefvttrFYrf/zxB25ubl=
x//fW8/vrrTJ48mT/++AMAX19fAIYPH86RI0dYuHAh1atX55tvvqF3795ERERw5ZVXsnXrVh5++=
GFefvll+vTpw88//+wIpUrDwIEDiY+PZ+3atbi5ufHUU08RFxdX4LiXX36Z1157jddff5133nmH=
+++/nyNHjhAUFFRqtZWrYKlt27Z8++23+fb9/PPPtGrVCjc3t3z7PT09qVGjBjk5OXz11Vfcfff=
dgJmutmzZkpUrV9K3b1/H8StXruT2228v/YcQkUrvp5/g/vshIQF27oTVq51dkYiIiIhI4fzwww=
+EhPwbgnXv3p1PPvmEDz74gJo1a/Lmm29isVho2LAhsbGxTJgwgeeffx4XF3PCVIMGDZg6darj/=
EmTJtGiRQsmTZrk2DdnzhzCw8PZv38/YWFhvPfee7z55psMGDAAgPr163PjjTc6jh87dqxju06d=
Ouzdu5evvvrKESxFRUUxevRoGjZsCMCVV17pOD4gIACLxZKvz9KhQ4f4/PPPOXDgANWrVwdg9Oj=
RrFy5koULFzJp0iTee+89unXrxjPPPANAeHg4mzdvZuXKlRf9Hvbv37/ArKqsrCzHCK6z7dmzh1=
WrVrFt2zZatWoFwP/+9z/Cw8MLHDt48GD69+8PwNSpU3nnnXfYunUrN99880XrKi6nBkupqakcO=
HDA8T4yMpKdO3cSFBRE7dq1GTduHDExMSxcuBAwV4B79913eeqppxg2bBibNm1i7ty5LFmyxHGN=
LVu2EBMTQ4sWLYiJieGll17Cbrfz7LPPOo556qmneOCBB2jVqhVt27blgw8+4OjRozzyyCOX7+F=
FpNKx22HKFHjpJcgbcbxxI2RkgJeXU0sTERERESfydvMmfnT8xQ8spXsXRceOHXn77bf/Pd/bPH=
/Pnj20adMmX4uZtm3bkpqaSnR0NLVr1wbgurOG6+/YsYN169blC6vyHDp0iKSkJLKysujcufN5a=
1q6dCnvvvsuhw4dIjU1ldzc3HwrmY0cOZIRI0bwySef0LlzZ/r160f9+vXPe70dO3ZgGAbNmjXL=
tz8rK8sx8mfv3r307t073+dt2rQpVLD05ptv0rVr13z7nnvuOWw22zmP37t3L66urvm+d1deeSW=
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
IJsRgiYiIiIiIiKgePD09ERMTA39/fyQmJsJsNsPDwwPe3t4uvTTKleh0OgQEBFTpYkpKSoKbm5=
vSpTUZBktERERERERE9aRSqeDn5wej0Yj09HQkJCQgJSUFJpMJHh4eSpdHTcTNzQ3e3t7w9vaGp=
6cnSkpKXCZcZLBEREREREREdIk0Gg2Cg4Ph4+OD5ORkJCcnw2KxcP6SC3J3d+dSOCIiIiIiIiKq=
O3d3d0RGRsLPzw9JSUlITU2FRqOBj4+PSy2PItfBYImIiIiIiIiogXl7e8PLywsBAQFISEhAamo=
qPD094e3trXRpRA2KwRIRERERERFRI6g8f8lsNiMhIQHJycmcv0ROhcESERERERERUSPSaDQICQ=
mpMn8pJycHvr6+0Gq1SpdHdEkYLBERERERERE1Ab1ej6ioKPj7+yMhIQFpaWnQarWcv0QOjb+5R=
ERERERERE3I29sbbdq0Qfv27WEwGJCSkoKcnBylyyKqF3YsERERERERETUxlUoFf39/mEwmpKWl=
lc9f8vHxgV6vV7o8olpjsERERERERESkEI1Gg9DQUPj6+iIpKam8e8nHx4fzl8ghMFgiIiIiIiI=
iUpher0d0dDT8/f2RmJjI+UvkMBgsEREREREREdkJo9EILy8vBAQEICEhAampqfDy8oKXl5fSpR=
HViMESERERERERkR1xc3NDQEBA+fylxMREpKSkwGQycf4S2R0GS0RERERERER2SKvVIiwsrMr8J=
YvFAj8/P2g0fDpP9oG/iURERERERER2zMPDAy1atCifv2Q2m6HT6eDj4wOVSqV0eeTiGCwRERER=
EREROQCTyQRvb28EBgYiISEBKSkpnL9EiuNoeSIiIiIiIiIHUTZ/qX379mjZsiWsViuSk5NRWFi=
odGnkotixRERERERERORgtFotmjVrBl9fXyQnJyM5ORkWiwW+vr6cv0RNir9tRERERERERA7KYD=
CUz19KSEhAeno63N3dYTKZOH+JmgSDJSIiIiIiIiIHVzZ/KT09nfOXqElxxhIRERERERGRE3Bzc=
0NgYCDat2+PFi1aoKSkBCkpKSgqKlK6NHJi7FgiIiIiIiIiciI6nQ7NmzeHn58fEhMTkZqaCgDw=
8fHh/CVqcPyNIiIiIiIiInJCBoMBLVu2REBAABITEzl/iRoFgyUiIiIiIiIiJ6VSqeDj41M+f+n=
06dNISUmBu7s7jEYj1Gq10iWSg2OwREREREREROTk1Go1goKC4Ovri8zMTKSkpMBsNkOtVsNoNE=
Kn0yldIjkoBktERERERERELkKr1SIoKAj+/v7Izs5GamoqMjIyYLVaYTQa4eHhoXSJ5GAYLBERE=
RERERG5GLVaDT8/P/j6+iInJwdmsxlpaWnIzs6Gl5cXPD09OYeJaoXBEhEREREREZGLUqlUMBqN=
MBqNCAkJQUZGBlJSUpCSkgK9Xg9vb2/OYaILYrBERERERERERDAYDDAYDAgKCkJmZiaSk5NhNpu=
h0WhgNBqh1WqVLpHsEIMlIiIiIiIiIiqn0+kQHByMgIAAZGVlISUlBZmZmbDZbDAajdDr9UqXSH=
aEwRIRERERERERVaNWq+Hv7w8/Pz9YLBakpaUhPT0dWVlZnMNE5RgsEREREREREdF5qVQqmEwmm=
EwmhIaGIj09HampqUhJSYGHhwe8vb3h5uamdJmkEAZLRERERERERFQrnp6e8PT0RHBwcPkcptTU=
VOh0OhiNRmg0jBlcDX/iRERERERERFQn7u7uCAkJqXEOk4+PD3Q6ndIlUhNhsERERERERERE9aL=
RaBAQEFA+hyk1NRXp6ekoKSmBt7c3DAaD0iVSI2OwRERERERERESXxM3NDT4+PvDx8UFOTk75HC=
aLxQJPT094eXlx0LeTYrBERERERERERA3G29sb3t7eCAkJQXp6OlJSUpCSkgJ3d3cYjUao1WqlS=
6QGxGCJiIiIiIiIiBqcXq9Hs2bNEBQUhMzMTKSkpMBsNkOtVsNoNHIOk5NgsEREREREREREjUar=
1SIoKAj+/v7Izs5GamoqMjIyYLVaYTQa4eHhoXSJdAkYLBERERERERFRo1Or1fDz84Ovry9ycnJ=
gNpuRlpaG7OxseHl5wdPTk3OYHBCDJSIiIiIiIiJqMiqVCkajEUajESEhIcjIyCifw6TX6+Ht7c=
05TA6EwRIRERERERERKcJgMMBgMJTPYUpOTobZbIZGo4HRaIRWq1W6RLoIBktEREREREREpCidT=
ofg4GAEBAQgKysLKSkpyMzMhM1mg9FohF6vV7pEOg8GS0RERERERERkF9RqNfz9/eHn5weLxYK0=
tDSkp6cjOzsbnp6enMNkhxgsEREREREREZFdUalUMJlMMJlMCA0NRWZmZvkcJp1OB6PRCI2GkYY=
94E+BiIiIiIiIiOxWWadSUFAQsrKykJqaioyMDADgMjk7wGCJiIiIiIiIiOyeTqdDUFAQAgICYL=
FYYDabuUzODjBYIiIiIiIiIiKH4ebmBh8fH/j4+HCZnB3gd5qIiIiIiIiIHNL5lsmpVCp4e3tzm=
VwTYLBERERERERERA7tfMvksrKy4OXlxWVyjYjBEhERERERERE5hZqWyaWmpnKZXCPid5OIiIiI=
iIiInE7lZXLZ2dlISUnhMrlGwGCJiIiIiIiIiJyWTqdDYGAg/P39uUyuETBYIiIiIiIiIiKnV3m=
ZXFhYGDIyMrhMrgHwO0ZERERERERELsVgMMBgMCA4OBhZWVlcJncJGCwRERERERERkUvSarXnXS=
bn6ekJLy8vLpO7CAZLREREREREROTSuEyu/vhdISIiIiIiIiI663zL5ADAaDRymdw53JT84ps3b=
8aQIUMQFhYGlUqFlStXXvRjNm3ahK5du0Kv16NFixZYtGhRtetkZWXh0UcfRWhoKPR6Pdq1a4c1=
a9aUv3/q1KlQqVRVTiEhIQ1504iIiIiIiIjIgZUtk2vfvj06duyIkJAQ5OfnIzk5GTk5ObDZbEq=
XaBcU7VjKzc1F586dce+992LYsGEXvf7x48dx44034oEHHsCnn36KrVu34pFHHkFgYGD5xxcVFW=
HAgAEICgrC119/jebNm+PUqVPw9vau8rk6dOiAX375pfyyWq1u2BtHRERERERERA7vfMvkUlNTo=
dVq4e3tDa1Wq3SZilE0WBo8eDAGDx5c6+svWrQIERERePPNNwEA7dq1w86dO/H666+XB0tLlixB=
RkYGfv/99/IfbGRkZLXPpdFo2KVERERERERERLV27jK51NRUZGZmAgC8vb3h4eGhcIVNT9GlcHW=
1bds2DBw4sMqxQYMGYefOnSguLgYArFq1Cr1798ajjz6K4OBgdOzYETNmzIDVaq3ycUeOHEFYWB=
iio6MRGxuLY8eOXfBrFxYWwmKxVDkRERERERERkespWybXrl07dOrUCSEhISgoKEBycjLy8vKUL=
q9JOVSwlJycjODg4CrHgoODUVJSArPZDAA4duwYvv76a1itVqxZswZTpkzB3LlzMX369PKP6dmz=
J5YtW4a1a9figw8+QHJyMq688kqkp6ef92vPnDkTJpOp/BQeHt44N5KIiIiIiIiIHIKbmxtMJhN=
iYmLQqVMntGzZEgaDwaWWxjncrnAqlarK5bJhWWXHS0tLERQUhPfffx9qtRpdu3ZFYmIi5syZgx=
dffBEAqiy/69SpE3r37o2WLVvi448/xvjx42v8upMmTaryPovFwnCJiIiIiIiIiABULJMLCgpCc=
XFxtfzCWTlUsBQSEoLk5OQqx1JTU6HRaODv7w8ACA0NhVarrTKMu127dkhOTkZRURF0Ol21z+vp=
6YlOnTrhyJEj5/3a7u7ucHd3b6BbQkRERERERETOSKvVulTHkkMthevduzfi4uKqHFu3bh26det=
W/kO76qqrcPToUZSWlpZf5/DhwwgNDa0xVAJkftLBgwcRGhraeMUTERERERERETkZRYOlM2fOYM=
+ePdizZw8A4Pjx49izZw/i4+MByPKzUaNGlV9/7NixOHnyJMaPH4+DBw9iyZIlWLx4MSZMmFB+n=
Ycffhjp6el48skncfjwYfz444+YMWMGHn300fLrTJgwAZs2bcLx48exfft23HHHHbBYLBg9enTT=
3HAiIiIiIiIiIieg6FK4nTt3ol+/fuWXy2YYjR49Gh999BGSkpLKQyYAiI6Oxpo1azBu3Di8884=
7CAsLw/z58zFs2LDy64SHh2PdunUYN24cLrvsMjRr1gxPPvkkJk6cWH6d06dP46677oLZbEZgYC=
B69eqFP/74A5GRkU1wq4mIiIiIiIiInIPKVjb9murEYrHAZDIhOzsbRqNR6XKIiIiIiIiIiBpEX=
TIPh5qxRERERERERERE9oPBEhERERERERER1QuDJSIiIiIiIiIiqhcGS0REREREREREVC8MloiI=
iIiIiIiIqF4YLBERERERERERUb0wWCIiIiIiIiIionphsERERERERERERPXCYImIiIiIiIiIiOq=
FwRIREREREREREdULgyUiIiIiIiIiIqoXBktERERERERERFQvDJaIiIiIiIiIiKheGCwRERERER=
EREVG9MFgiIiIiIiIiIqJ6YbBERERERERERET1wmCJiIiIiIiIiIjqRaN0AY7KZrMBACwWi8KVE=
BERERERERE1nLKsoyz7uBAGS/WUk5MDAAgPD1e4EiIiIiIiIiKihpeTkwOTyXTB66hstYmfqJrS=
0lIkJibC29sbKpVK6XLqxWKxIDw8HKdOnYLRaFS6HCKXw79BIuXw749IOfz7I1IO//6otmw2G3J=
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
b5s+fjwMHDuDjjz/G+vXr8eyzzwIAPD09ERsbi6VLl1b5HEuXLsUdd9wBb2/vJq+fiIiIXIvKZr=
PZlC6CiIiIyNWMGTMGWVlZWLlyZbX3xcbGYt++ffjnn3+qve+rr77Cww8/DLPZDADYsWMHrrzyS=
sTHxyMsLAxmsxlhYWGIi4tD3759G/tmEBERkYtjxxIRERGRnbHZbFCpVACADRs2YMCAAWjWrBm8=
vb0xatQopKenIzc3FwDQo0cPdOjQAcuWLQMAfPLJJ4iIiECfPn0Uq5+IiIhcB4MlIiIiIjtz8OB=
BREdH4+TJk7jxxhvRsWNHfPPNN9i1axfeeecdAEBxcXH59e+///7y5XBLly7FvffeWx5MERERET=
UmBktEREREdmT9+vXYv38/hg0bhp07d6KkpARz585Fr1690Lp1ayQmJlb7mJEjRyI+Ph7z58/H3=
3//jdGjRytQOREREbkijdIFEBEREbmqwsJCJCcnw2q1IiUlBT///DNmzpyJm2++GaNGjcL+/ftR=
UlKCt99+G0OGDMHWrVuxaNGiap/H19cXt99+O5555hkMHDgQzZs3V+DWEBERkStixxIRERGRQn7=
++WeEhoYiKioKN9xwAzZs2ID58+fj+++/h1qtxuWXX4433ngDs2bNQseOHbF8+XLMnDmzxs/1v/=
/9D0VFRbjvvvua+FYQERGRK+OucEREREROYPny5XjyySeRmJgInU6ndDlERETkIrgUjoiIiMiB5=
eXl4fjx45g5cyYeeughhkpERETUpLgUjoiIiMiBzZ49G5dffjmCg4MxadIkpcshIiIiF8OlcERE=
REREREREVC/sWCIiIiIiIiIionphsERERERERERERPXCYImIiIiIiIiIiOqFwRIREREREREREdU=
LgyUiIiIiIiIiIqoXBktERERERERERFQvDJaIiIiIiIiIiKheGCwREREREREREVG9/D+u+r/cur=
EcOwAAAABJRU5ErkJggg=3D=3D"></div></div></div><div class=3D"btn btn-default=
 output_collapsed" title=3D"click to expand output" style=3D"display: none;=
">. . .</div></div></div><div class=3D"cell code_cell rendered selected" ta=
bindex=3D"2"><div class=3D"input"><div class=3D"prompt_container"><div clas=
s=3D"prompt input_prompt"><bdi>In</bdi>&nbsp;[27]:</div><div class=3D"run_t=
his_cell" title=3D"Run this cell"><i class=3D"fa-step-forward fa"></i></div=
></div><div class=3D"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"=
celltoolbar"></div></div><div class=3D"input_area" aria-label=3D"Edit code =
here"><div class=3D"CodeMirror cm-s-ipython"><div style=3D"overflow: hidden=
; position: relative; width: 3px; height: 0px; top: 22.6px; left: 145.769px=
;"><textarea autocorrect=3D"off" autocapitalize=3D"off" spellcheck=3D"false=
" tabindex=3D"0" style=3D"position: absolute; bottom: -1em; padding: 0px; w=
idth: 1000px; height: 1em; outline: none;"></textarea></div><div class=3D"C=
odeMirror-vscrollbar" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D=
"min-width: 1px; height: 0px;"></div></div><div class=3D"CodeMirror-hscroll=
bar" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"height: 100%; mi=
n-height: 1px; width: 0px;"></div></div><div class=3D"CodeMirror-scrollbar-=
filler" cm-not-content=3D"true"></div><div class=3D"CodeMirror-gutter-fille=
r" cm-not-content=3D"true"></div><div class=3D"CodeMirror-scroll" tabindex=
=3D"-1"><div class=3D"CodeMirror-sizer" style=3D"margin-left: 34px; min-wid=
th: 384.175px; margin-bottom: -17px; border-right-width: 33px; min-height: =
45px; padding-right: 0px; padding-bottom: 0px;"><div style=3D"position: rel=
ative; top: 0px;"><div class=3D"CodeMirror-lines" role=3D"presentation"><di=
v role=3D"presentation" style=3D"position: relative; outline: none;"><div c=
lass=3D"CodeMirror-measure"><pre class=3D"CodeMirror-line-like">x</pre></di=
v><div class=3D"CodeMirror-measure"></div><div style=3D"position: relative;=
 z-index: 1;"><div class=3D"CodeMirror-selected" style=3D"position: absolut=
e; left: 4px; top: 0px; width: 580px; height: 17px;"></div><div class=3D"Co=
deMirror-selected" style=3D"position: absolute; left: 4px; top: 17px; width=
: 107.769px; height: 17px;"></div></div><div class=3D"CodeMirror-cursors" s=
tyle=3D""></div><div class=3D"CodeMirror-code" role=3D"presentation"><div s=
tyle=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" style=
=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt=
" style=3D"left: 0px; width: 21px;">1</div></div><pre class=3D" CodeMirror-=
line " role=3D"presentation"><span role=3D"presentation" style=3D"padding-r=
ight: 0.1px;"><span class=3D"cm-builtin">print</span>(<span class=3D"cm-str=
ing">"The mse of the (Low, High) forcasting is"</span>)</span></pre></div><=
div style=3D"position: relative;"><div class=3D"CodeMirror-gutter-wrapper" =
style=3D"left: -34px;"><div class=3D"CodeMirror-linenumber CodeMirror-gutte=
r-elt" style=3D"left: 0px; width: 21px;">2</div></div><pre class=3D" CodeMi=
rror-line " role=3D"presentation"><span role=3D"presentation" style=3D"padd=
ing-right: 0.1px;"><span class=3D"cm-builtin">print</span>(<span class=3D"c=
m-variable">forcast</span>)</span></pre></div></div></div></div></div></div=
><div style=3D"position: absolute; height: 33px; width: 1px; border-bottom:=
 0px solid transparent; top: 45px;"></div><div class=3D"CodeMirror-gutters"=
 style=3D"height: 78px; left: 0px;"><div class=3D"CodeMirror-gutter CodeMir=
ror-linenumbers" style=3D"width: 33px;"></div></div></div></div></div></div=
></div><div class=3D"output_wrapper"><div class=3D"out_prompt_overlay promp=
t" title=3D"click to scroll output; double click to hide"></div><div class=
=3D"output"><div class=3D"output_area"><div class=3D"run_this_cell"></div><=
div class=3D"prompt"></div><div class=3D"output_subarea output_text output_=
stream output_stdout" dir=3D"auto"><pre>The mse of the (Low, High) forcasti=
ng is
[0.004799886196411286, 0.0032559867677543057]
</pre></div></div></div><div class=3D"btn btn-default output_collapsed" tit=
le=3D"click to expand output" style=3D"display: none;">. . .</div></div></d=
iv><div class=3D"cell code_cell unrendered unselected" tabindex=3D"2"><div =
class=3D"input"><div class=3D"prompt_container"><div class=3D"prompt input_=
prompt"><bdi>In</bdi>&nbsp;[&nbsp;]:</div><div class=3D"run_this_cell" titl=
e=3D"Run this cell"><i class=3D"fa-step-forward fa"></i></div></div><div cl=
ass=3D"inner_cell"><div class=3D"ctb_hideshow"><div class=3D"celltoolbar"><=
/div></div><div class=3D"input_area" aria-label=3D"Edit code here"><div cla=
ss=3D"CodeMirror cm-s-ipython"><div style=3D"overflow: hidden; position: re=
lative; width: 3px; height: 0px; top: 5.6001px; left: 38px;"><textarea auto=
correct=3D"off" autocapitalize=3D"off" spellcheck=3D"false" tabindex=3D"0" =
style=3D"position: absolute; bottom: -1em; padding: 0px; width: 1000px; hei=
ght: 1em; outline: none;"></textarea></div><div class=3D"CodeMirror-vscroll=
bar" tabindex=3D"-1" cm-not-content=3D"true"><div style=3D"min-width: 1px; =
height: 0px;"></div></div><div class=3D"CodeMirror-hscrollbar" tabindex=3D"=
-1" cm-not-content=3D"true"><div style=3D"height: 100%; min-height: 1px; wi=
dth: 0px;"></div></div><div class=3D"CodeMirror-scrollbar-filler" cm-not-co=
ntent=3D"true"></div><div class=3D"CodeMirror-gutter-filler" cm-not-content=
=3D"true"></div><div class=3D"CodeMirror-scroll" tabindex=3D"-1"><div class=
=3D"CodeMirror-sizer" style=3D"margin-left: 34px; min-width: 7px; margin-bo=
ttom: -17px; border-right-width: 33px; min-height: 28px; padding-right: 0px=
; padding-bottom: 0px;"><div style=3D"position: relative; top: 0px;"><div c=
lass=3D"CodeMirror-lines" role=3D"presentation"><div role=3D"presentation" =
style=3D"position: relative; outline: none;"><div class=3D"CodeMirror-measu=
re"><div class=3D"CodeMirror-linenumber CodeMirror-gutter-elt"><div>1</div>=
</div></div><div class=3D"CodeMirror-measure"></div><div style=3D"position:=
 relative; z-index: 1;"></div><div class=3D"CodeMirror-cursors" style=3D"vi=
sibility: hidden;"><div class=3D"CodeMirror-cursor" style=3D"left: 4px; top=
: 0px; height: 17px;">&nbsp;</div></div><div class=3D"CodeMirror-code" role=
=3D"presentation"><div style=3D"position: relative;"><div class=3D"CodeMirr=
or-gutter-wrapper" style=3D"left: -34px;"><div class=3D"CodeMirror-linenumb=
er CodeMirror-gutter-elt" style=3D"left: 0px; width: 21px;">1</div></div><p=
re class=3D" CodeMirror-line " role=3D"presentation"><span role=3D"presenta=
tion" style=3D"padding-right: 0.1px;"><span cm-text=3D"">=E2=80=8B</span></=
span></pre></div></div></div></div></div></div><div style=3D"position: abso=
lute; height: 33px; width: 1px; border-bottom: 0px solid transparent; top: =
28px;"></div><div class=3D"CodeMirror-gutters" style=3D"height: 61px; left:=
 0px;"><div class=3D"CodeMirror-gutter CodeMirror-linenumbers" style=3D"wid=
th: 33px;"></div></div></div></div></div></div></div><div class=3D"output_w=
rapper"><div class=3D"out_prompt_overlay prompt" title=3D"click to expand o=
utput; double click to hide output"></div><div class=3D"output"></div><div =
class=3D"btn btn-default output_collapsed" title=3D"click to expand output"=
 style=3D"display: none;">. . .</div></div></div></div><div class=3D"end_sp=
ace"></div></div>
        <div id=3D"tooltip" class=3D"ipython_tooltip" style=3D"display:none=
"><div class=3D"tooltipbuttons"><a href=3D"http://localhost:8890/notebooks/=
Code%20for%20forecasting%20currency-crosses%20from%20investing.com%20#" rol=
e=3D"button" class=3D"ui-button"><span class=3D"ui-icon ui-icon-close">Clos=
e</span></a><a href=3D"http://localhost:8890/notebooks/Code%20for%20forecas=
ting%20currency-crosses%20from%20investing.com%20#" role=3D"button" class=
=3D"ui-button" id=3D"expanbutton" title=3D"Grow the tooltip vertically (pre=
ss shift-tab twice)"><span class=3D"ui-icon ui-icon-plus">Expand</span></a>=
<a href=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20curre=
ncy-crosses%20from%20investing.com%20#" role=3D"button" class=3D"ui-button"=
 title=3D"show the current docstring in pager (press shift-tab 4 times)"><s=
pan class=3D"ui-icon ui-icon-arrowstop-l-n">Open in Pager</span></a><a href=
=3D"http://localhost:8890/notebooks/Code%20for%20forecasting%20currency-cro=
sses%20from%20investing.com%20#" role=3D"button" class=3D"ui-button" title=
=3D"Tooltip will linger for 10 seconds while you type" style=3D"display: no=
ne;"><span class=3D"ui-icon ui-icon-clock">Close</span></a></div><div class=
=3D"pretooltiparrow"></div><div class=3D"tooltiptext smalltooltip"></div></=
div>
    </div>
</div>



</div>



<div id=3D"pager" class=3D"ui-resizable">
    <div id=3D"pager-contents">
        <div id=3D"pager-container" class=3D"container"></div>
    </div>
    <div id=3D"pager-button-area"><a role=3D"button" title=3D"Open the page=
r in an external window" class=3D"ui-button"><span class=3D"ui-icon ui-icon=
-extlink"></span></a><a role=3D"button" title=3D"Close the pager" class=3D"=
ui-button"><span class=3D"ui-icon ui-icon-close"></span></a></div>
<div class=3D"ui-resizable-handle ui-resizable-n" style=3D"z-index: 90;"></=
div></div>

















<div style=3D"position: absolute; width: 0px; height: 0px; overflow: hidden=
; padding: 0px; border: 0px; margin: 0px;"><div id=3D"MathJax_Font_Test" st=
yle=3D"position: absolute; visibility: hidden; top: 0px; left: 0px; width: =
auto; min-width: 0px; max-width: none; padding: 0px; border: 0px; margin: 0=
px; white-space: nowrap; text-align: left; text-indent: 0px; text-transform=
: none; line-height: normal; letter-spacing: normal; word-spacing: normal; =
font-size: 40px; font-weight: normal; font-style: normal;"></div></div></bo=
dy></html>
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-cf0de846-b81b-415b-b4ae-0efe32fe6a1f@mhtml.blink

@charset "utf-8";

.MathJax_Hover_Frame { border-radius: 0.25em; box-shadow: rgb(136, 51, 170)=
 0px 0px 15px; display: inline-block; position: absolute; border: 1px solid=
 rgb(170, 102, 221) !important; }

.MathJax_Menu_Button .MathJax_Hover_Arrow { position: absolute; cursor: poi=
nter; display: inline-block; border: 2px solid rgb(170, 170, 170); border-r=
adius: 4px; font-family: "Courier New", Courier; font-size: 9px; color: rgb=
(240, 240, 240); }

.MathJax_Menu_Button .MathJax_Hover_Arrow span { display: block; background=
-color: rgb(170, 170, 170); border: 1px solid; border-radius: 3px; line-hei=
ght: 0; padding: 4px; }

.MathJax_Hover_Arrow:hover { color: white !important; border: 2px solid rgb=
(204, 204, 204) !important; }

.MathJax_Hover_Arrow:hover span { background-color: rgb(204, 204, 204) !imp=
ortant; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-c3982157-b0ef-49d1-b6c6-bf731d1e50a4@mhtml.blink

@charset "utf-8";

#MathJax_About { position: fixed; left: 50%; width: auto; text-align: cente=
r; border: 3px outset; padding: 1em 2em; background-color: rgb(221, 221, 22=
1); color: black; cursor: default; font-family: message-box; font-size: 120=
%; font-style: normal; text-indent: 0px; text-transform: none; line-height:=
 normal; letter-spacing: normal; word-spacing: normal; overflow-wrap: norma=
l; white-space: nowrap; float: none; z-index: 201; border-radius: 15px; box=
-shadow: rgb(128, 128, 128) 0px 10px 20px; }

#MathJax_About.MathJax_MousePost { outline: none; }

.MathJax_Menu { position: absolute; background-color: white; color: black; =
width: auto; padding: 2px; border: 1px solid rgb(204, 204, 204); margin: 0p=
x; cursor: default; font-style: ; font-variant: normal; font-weight: ; font=
-stretch: ; font-size: ; font-family: ; font-optical-sizing: ; font-kerning=
: ; font-feature-settings: ; font-variation-settings: ; text-align: left; t=
ext-indent: 0px; text-transform: none; line-height: normal; letter-spacing:=
 normal; word-spacing: normal; overflow-wrap: normal; white-space: nowrap; =
float: none; z-index: 201; box-shadow: rgb(128, 128, 128) 0px 10px 20px; }

.MathJax_MenuItem { padding: 2px 2em; background: transparent; }

.MathJax_MenuArrow { position: absolute; right: 0.5em; padding-top: 0.25em;=
 color: rgb(102, 102, 102); font-size: 0.75em; }

.MathJax_MenuActive .MathJax_MenuArrow { color: white; }

.MathJax_MenuArrow.RTL { left: 0.5em; right: auto; }

.MathJax_MenuCheck { position: absolute; left: 0.7em; }

.MathJax_MenuCheck.RTL { right: 0.7em; left: auto; }

.MathJax_MenuRadioCheck { position: absolute; left: 1em; }

.MathJax_MenuRadioCheck.RTL { right: 1em; left: auto; }

.MathJax_MenuLabel { padding: 2px 2em 4px 1.33em; font-style: italic; }

.MathJax_MenuRule { border-top: 1px solid rgb(204, 204, 204); margin: 4px 1=
px 0px; }

.MathJax_MenuDisabled { color: graytext; }

.MathJax_MenuActive { background-color: highlight; color: highlighttext; }

.MathJax_MenuDisabled:focus, .MathJax_MenuLabel:focus { background-color: r=
gb(232, 232, 232); }

.MathJax_ContextMenu:focus { outline: none; }

.MathJax_ContextMenu .MathJax_MenuItem:focus { outline: none; }

#MathJax_AboutClose { top: 0.2em; right: 0.2em; }

.MathJax_Menu .MathJax_MenuClose { top: -10px; left: -10px; }

.MathJax_MenuClose { position: absolute; cursor: pointer; display: inline-b=
lock; border: 2px solid rgb(170, 170, 170); border-radius: 18px; font-famil=
y: "Courier New", Courier; font-size: 24px; color: rgb(240, 240, 240); }

.MathJax_MenuClose span { display: block; background-color: rgb(170, 170, 1=
70); border: 1.5px solid; border-radius: 18px; line-height: 0; padding: 8px=
 0px 6px; }

.MathJax_MenuClose:hover { color: white !important; border: 2px solid rgb(2=
04, 204, 204) !important; }

.MathJax_MenuClose:hover span { background-color: rgb(204, 204, 204) !impor=
tant; }

.MathJax_MenuClose:hover:focus { outline: none; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-b5b5bf9d-9255-45e7-bc73-7909123caf80@mhtml.blink

@charset "utf-8";

.MathJax_Preview .MJXf-math { color: inherit !important; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-d5fa4ba8-dd42-41b1-a3f6-e37c4ae43185@mhtml.blink

@charset "utf-8";

.MJX_Assistive_MathML { top: 0px; left: 0px; clip: rect(1px, 1px, 1px, 1px)=
; user-select: none; position: absolute !important; padding: 1px 0px 0px !i=
mportant; border: 0px !important; height: 1px !important; width: 1px !impor=
tant; overflow: hidden !important; display: block !important; }

.MJX_Assistive_MathML.MJX_Assistive_MathML_Block { width: 100% !important; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-75e0ea17-5bb2-43a3-9c86-5539cd4d9e14@mhtml.blink

@charset "utf-8";

#MathJax_Zoom { position: absolute; background-color: rgb(240, 240, 240); o=
verflow: auto; display: block; z-index: 301; padding: 0.5em; border: 1px so=
lid black; margin: 0px; font-weight: normal; font-style: normal; text-align=
: left; text-indent: 0px; text-transform: none; line-height: normal; letter=
-spacing: normal; word-spacing: normal; overflow-wrap: normal; white-space:=
 nowrap; float: none; box-sizing: content-box; box-shadow: rgb(170, 170, 17=
0) 5px 5px 15px; }

#MathJax_ZoomOverlay { position: absolute; left: 0px; top: 0px; z-index: 30=
0; display: inline-block; width: 100%; height: 100%; border: 0px; padding: =
0px; margin: 0px; background-color: white; opacity: 0; }

#MathJax_ZoomFrame { position: relative; display: inline-block; height: 0px=
; width: 0px; }

#MathJax_ZoomEventTrap { position: absolute; left: 0px; top: 0px; z-index: =
302; display: inline-block; border: 0px; padding: 0px; margin: 0px; backgro=
und-color: white; opacity: 0; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-96a39898-bcc9-48ae-9d83-74b6eb3afb0d@mhtml.blink

@charset "utf-8";

.MathJax_Preview { color: rgb(136, 136, 136); display: contents; }

#MathJax_Message { position: fixed; left: 1em; bottom: 1.5em; background-co=
lor: rgb(230, 230, 230); border: 1px solid rgb(149, 149, 149); margin: 0px;=
 padding: 2px 8px; z-index: 102; color: black; font-size: 80%; width: auto;=
 white-space: nowrap; }

#MathJax_MSIE_Frame { position: absolute; top: 0px; left: 0px; width: 0px; =
z-index: 101; border: 0px; margin: 0px; padding: 0px; }

.MathJax_Error { color: rgb(204, 0, 0); font-style: italic; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-57dffdf9-e0fd-4707-a914-03051e14c18b@mhtml.blink

@charset "utf-8";

div.MathJax_MathML { text-align: center; margin: 0.75em 0px; display: block=
 !important; }

.MathJax_MathML { font-style: normal; font-weight: normal; line-height: nor=
mal; font-size: 100%; text-indent: 0px; text-align: left; text-transform: n=
one; letter-spacing: normal; word-spacing: normal; overflow-wrap: normal; w=
hite-space: nowrap; float: none; direction: ltr; max-width: none; max-heigh=
t: none; min-width: 0px; min-height: 0px; border: 0px; padding: 0px; margin=
: 0px; }

span.MathJax_MathML { display: inline !important; }

.MathJax_mmlExBox { overflow: hidden; height: 1px; width: 60ex; min-height:=
 0px; max-height: none; padding: 0px; border: 0px; margin: 0px; display: bl=
ock !important; }

[class=3D"MJX-tex-oldstyle"] { font-family: MathJax_Caligraphic, MathJax_Ca=
ligraphic-WEB; }

[class=3D"MJX-tex-oldstyle-bold"] { font-family: MathJax_Caligraphic, MathJ=
ax_Caligraphic-WEB; font-weight: bold; }

[class=3D"MJX-tex-caligraphic"] { font-family: MathJax_Caligraphic, MathJax=
_Caligraphic-WEB; }

[class=3D"MJX-tex-caligraphic-bold"] { font-family: MathJax_Caligraphic, Ma=
thJax_Caligraphic-WEB; font-weight: bold; }

@font-face { font-family: MathJax_Caligraphic-WEB; src: url("http://localho=
st:8890/static/components/MathJax/fonts/HTML-CSS/TeX/otf/MathJax_Caligraphi=
c-Regular.otf"); }

@font-face { font-family: MathJax_Caligraphic-WEB; font-weight: bold; src: =
url("http://localhost:8890/static/components/MathJax/fonts/HTML-CSS/TeX/otf=
/MathJax_Caligraphic-Bold.otf"); }

[mathvariant=3D"double-struck"] { font-family: MathJax_AMS, MathJax_AMS-WEB=
; }

[mathvariant=3D"script"] { font-family: MathJax_Script, MathJax_Script-WEB;=
 }

[mathvariant=3D"fraktur"] { font-family: MathJax_Fraktur, MathJax_Fraktur-W=
EB; }

[mathvariant=3D"bold-script"] { font-family: MathJax_Script, MathJax_Caligr=
aphic-WEB; font-weight: bold; }

[mathvariant=3D"bold-fraktur"] { font-family: MathJax_Fraktur, MathJax_Frak=
tur-WEB; font-weight: bold; }

[mathvariant=3D"monospace"] { font-family: monospace; }

[mathvariant=3D"sans-serif"] { font-family: sans-serif; }

[mathvariant=3D"bold-sans-serif"] { font-family: sans-serif; font-weight: b=
old; }

[mathvariant=3D"sans-serif-italic"] { font-family: sans-serif; font-style: =
italic; }

[mathvariant=3D"sans-serif-bold-italic"] { font-family: sans-serif; font-st=
yle: italic; font-weight: bold; }

@font-face { font-family: MathJax_AMS-WEB; src: url("http://localhost:8890/=
static/components/MathJax/fonts/HTML-CSS/TeX/otf/MathJax_AMS-Regular.otf");=
 }

@font-face { font-family: MathJax_Script-WEB; src: url("http://localhost:88=
90/static/components/MathJax/fonts/HTML-CSS/TeX/otf/MathJax_Script-Regular.=
otf"); }

@font-face { font-family: MathJax_Fraktur-WEB; src: url("http://localhost:8=
890/static/components/MathJax/fonts/HTML-CSS/TeX/otf/MathJax_Fraktur-Regula=
r.otf"); }

@font-face { font-family: MathJax_Fraktur-WEB; font-weight: bold; src: url(=
"http://localhost:8890/static/components/MathJax/fonts/HTML-CSS/TeX/otf/Mat=
hJax_Fraktur-Bold.otf"); }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-46264988-c362-4058-a17a-20d3ea3c46ca@mhtml.blink

@charset "utf-8";

.MJXp-script { font-size: 0.8em; }

.MJXp-right { transform-origin: right center; }

.MJXp-bold { font-weight: bold; }

.MJXp-italic { font-style: italic; }

.MJXp-scr { font-family: MathJax_Script, "Times New Roman", Times, STIXGene=
ral, serif; }

.MJXp-frak { font-family: MathJax_Fraktur, "Times New Roman", Times, STIXGe=
neral, serif; }

.MJXp-sf { font-family: MathJax_SansSerif, "Times New Roman", Times, STIXGe=
neral, serif; }

.MJXp-cal { font-family: MathJax_Caligraphic, "Times New Roman", Times, STI=
XGeneral, serif; }

.MJXp-mono { font-family: MathJax_Typewriter, "Times New Roman", Times, STI=
XGeneral, serif; }

.MJXp-largeop { font-size: 150%; }

.MJXp-largeop.MJXp-int { vertical-align: -0.2em; }

.MJXp-math { display: inline-block; line-height: 1.2; text-indent: 0px; fon=
t-family: "Times New Roman", Times, STIXGeneral, serif; white-space: nowrap=
; border-collapse: collapse; }

.MJXp-display { display: block; text-align: center; margin: 1em 0px; }

.MJXp-math span { display: inline-block; }

.MJXp-box { text-align: center; display: block !important; }

.MJXp-box::after { content: " "; }

.MJXp-rule { margin-top: 0.1em; display: block !important; }

.MJXp-char { display: block !important; }

.MJXp-mo { margin: 0px 0.15em; }

.MJXp-mfrac { margin: 0px 0.125em; vertical-align: 0.25em; }

.MJXp-denom { width: 100%; display: inline-table !important; }

.MJXp-denom > * { display: table-row !important; }

.MJXp-surd { vertical-align: top; }

.MJXp-surd > * { display: block !important; }

.MJXp-script-box > * { height: 50%; display: table !important; }

.MJXp-script-box > * > * { vertical-align: top; display: table-cell !import=
ant; }

.MJXp-script-box > :last-child > * { vertical-align: bottom; }

.MJXp-script-box > * > * > * { display: block !important; }

.MJXp-mphantom { visibility: hidden; }

.MJXp-munderover, .MJXp-munder { display: inline-table !important; }

.MJXp-over { text-align: center; display: inline-block !important; }

.MJXp-over > * { display: block !important; }

.MJXp-munderover > *, .MJXp-munder > * { display: table-row !important; }

.MJXp-mtable { vertical-align: 0.25em; margin: 0px 0.125em; }

.MJXp-mtable > * { vertical-align: middle; display: inline-table !important=
; }

.MJXp-mtr { display: table-row !important; }

.MJXp-mtd { text-align: center; padding: 0.5em 0px 0px 0.5em; display: tabl=
e-cell !important; }

.MJXp-mtr > .MJXp-mtd:first-child { padding-left: 0px; }

.MJXp-mtr:first-child > .MJXp-mtd { padding-top: 0px; }

.MJXp-mlabeledtr { display: table-row !important; }

.MJXp-mlabeledtr > .MJXp-mtd:first-child { padding-left: 0px; }

.MJXp-mlabeledtr:first-child > .MJXp-mtd { padding-top: 0px; }

.MJXp-merror { background-color: rgb(255, 255, 136); color: rgb(204, 0, 0);=
 border: 1px solid rgb(204, 0, 0); padding: 1px 3px; font-style: normal; fo=
nt-size: 90%; }

.MJXp-scale0 { transform: scaleX(0); }

.MJXp-scale1 { transform: scaleX(0.1); }

.MJXp-scale2 { transform: scaleX(0.2); }

.MJXp-scale3 { transform: scaleX(0.3); }

.MJXp-scale4 { transform: scaleX(0.4); }

.MJXp-scale5 { transform: scaleX(0.5); }

.MJXp-scale6 { transform: scaleX(0.6); }

.MJXp-scale7 { transform: scaleX(0.7); }

.MJXp-scale8 { transform: scaleX(0.8); }

.MJXp-scale9 { transform: scaleX(0.9); }

.MathJax_PHTML .noError { font-size: 90%; text-align: left; color: black; p=
adding: 1px 3px; border: 1px solid; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-0bfb7d94-ed8f-4684-ac25-c9e5b1abb8f3@mhtml.blink

@charset "utf-8";

.MathJax_Display { text-align: center; margin: 0px; position: relative; tex=
t-indent: 0px; max-width: none; max-height: none; min-width: 0px; min-heigh=
t: 0px; width: 100%; display: block !important; }

.MathJax .merror { background-color: rgb(255, 255, 136); color: rgb(204, 0,=
 0); border: 1px solid rgb(204, 0, 0); padding: 1px 3px; font-style: normal=
; font-size: 90%; }

.MathJax .MJX-monospace { font-family: monospace; }

.MathJax .MJX-sans-serif { font-family: sans-serif; }

#MathJax_Tooltip { background-color: infobackground; color: infotext; borde=
r: 1px solid black; box-shadow: rgb(170, 170, 170) 2px 2px 5px; padding: 3p=
x 4px; z-index: 401; position: absolute; left: 0px; top: 0px; width: auto; =
height: auto; display: none; }

.MathJax { display: inline; font-style: normal; font-weight: normal; line-h=
eight: normal; font-size: 100%; text-indent: 0px; text-align: left; text-tr=
ansform: none; letter-spacing: normal; word-spacing: normal; overflow-wrap:=
 normal; white-space: nowrap; float: none; direction: ltr; max-width: none;=
 max-height: none; min-width: 0px; min-height: 0px; border: 0px; padding: 0=
px; margin: 0px; }

.MathJax:focus, body :focus .MathJax { display: inline-table; }

.MathJax.MathJax_FullWidth { text-align: center; display: table-cell !impor=
tant; width: 10000em !important; }

.MathJax img, .MathJax nobr, .MathJax a { border: 0px; padding: 0px; margin=
: 0px; max-width: none; max-height: none; min-width: 0px; min-height: 0px; =
vertical-align: 0px; line-height: normal; text-decoration: none; }

img.MathJax_strut { border: 0px !important; padding: 0px !important; margin=
: 0px !important; vertical-align: 0px !important; }

.MathJax span { display: inline; position: static; border: 0px; padding: 0p=
x; margin: 0px; vertical-align: 0px; line-height: normal; text-decoration: =
none; box-sizing: content-box; }

.MathJax nobr { white-space: nowrap !important; }

.MathJax img { display: inline !important; float: none !important; }

.MathJax * { transition: none 0s ease 0s; }

.MathJax_Processing { visibility: hidden; position: fixed; width: 0px; heig=
ht: 0px; overflow: hidden; }

.MathJax_Processed { display: none !important; }

.MathJax_test { font-style: normal; font-weight: normal; font-size: 100%; t=
ext-indent: 0px; text-transform: none; letter-spacing: normal; word-spacing=
: normal; overflow: hidden; height: 1px; }

.MathJax_test.mjx-test-display { display: table !important; }

.MathJax_test.mjx-test-inline { margin-right: -1px; display: inline !import=
ant; }

.MathJax_test.mjx-test-default { clear: both; display: block !important; }

.MathJax_ex_box { position: absolute; overflow: hidden; min-height: 0px; ma=
x-height: none; padding: 0px; border: 0px; margin: 0px; width: 1px; height:=
 60ex; display: inline-block !important; }

.MathJax_em_box { position: absolute; overflow: hidden; min-height: 0px; ma=
x-height: none; padding: 0px; border: 0px; margin: 0px; width: 1px; height:=
 60em; display: inline-block !important; }

.mjx-test-inline .MathJax_left_box { display: inline-block; width: 0px; flo=
at: left; }

.mjx-test-inline .MathJax_right_box { display: inline-block; width: 0px; fl=
oat: right; }

.mjx-test-display .MathJax_right_box { min-width: 0px; max-width: none; pad=
ding: 0px; border: 0px; margin: 0px; display: table-cell !important; width:=
 10000em !important; }

.MathJax .MathJax_HitBox { cursor: text; background: white; opacity: 0; }

.MathJax .MathJax_HitBox * { filter: none; opacity: 1; background: transpar=
ent; }

#MathJax_Tooltip * { filter: none; opacity: 1; background: transparent; }

@font-face { font-family: MathJax_Blank; src: url("about:blank"); }

.MathJax .noError { font-size: 90%; text-align: left; color: black; padding=
: 1px 3px; border: 1px solid; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-854fd570-7fde-4c96-a903-98e468bbaec8@mhtml.blink

@charset "utf-8";

.jupyter-widgets-output-area div.output_subarea { max-width: 100%; }

.jupyter-widgets-output-area > .out_prompt_overlay { display: none; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-7fce1f8c-a4bc-4861-a819-2a17277aa1bb@mhtml.blink

@charset "utf-8";

.p-Widget, .lm-Widget { box-sizing: border-box; position: relative; overflo=
w: hidden; cursor: default; }

.p-Widget.p-mod-hidden, .lm-Widget.lm-mod-hidden { display: none !important=
; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-54248245-f784-467f-8808-bac75ad7fe78@mhtml.blink

@charset "utf-8";

.lm-AccordionPanel[data-orientation=3D"horizontal"] > .lm-AccordionPanel-ti=
tle { display: block; transform-origin: left top; transform: rotate(-90deg)=
 translate(-100%); }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-3ba88621-bb13-4404-9787-bdcb6456eb83@mhtml.blink

@charset "utf-8";

.p-CommandPalette, .lm-CommandPalette { display: flex; flex-direction: colu=
mn; user-select: none; }

.p-CommandPalette-search, .lm-CommandPalette-search { flex: 0 0 auto; }

.p-CommandPalette-content, .lm-CommandPalette-content { flex: 1 1 auto; mar=
gin: 0px; padding: 0px; min-height: 0px; overflow: auto; list-style-type: n=
one; }

.p-CommandPalette-header, .lm-CommandPalette-header { overflow: hidden; whi=
te-space: nowrap; text-overflow: ellipsis; }

.p-CommandPalette-item, .lm-CommandPalette-item { display: flex; flex-direc=
tion: row; }

.p-CommandPalette-itemIcon, .lm-CommandPalette-itemIcon { flex: 0 0 auto; }

.p-CommandPalette-itemContent, .lm-CommandPalette-itemContent { flex: 1 1 a=
uto; overflow: hidden; }

.p-CommandPalette-itemShortcut, .lm-CommandPalette-itemShortcut { flex: 0 0=
 auto; }

.p-CommandPalette-itemLabel, .lm-CommandPalette-itemLabel { overflow: hidde=
n; white-space: nowrap; text-overflow: ellipsis; }

.lm-close-icon { border: 1px solid transparent; background-color: transpare=
nt; position: absolute; z-index: 1; right: 3%; top: 0px; bottom: 0px; margi=
n: auto; padding: 7px 0px; display: none; vertical-align: middle; outline: =
0px; cursor: pointer; }

.lm-close-icon::after { content: "X"; display: block; width: 15px; height: =
15px; text-align: center; color: rgb(0, 0, 0); font-weight: normal; font-si=
ze: 12px; cursor: pointer; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-444b85d2-0450-4409-a3de-3e2c0d9f1571@mhtml.blink

@charset "utf-8";

.p-DockPanel, .lm-DockPanel { z-index: 0; }

.p-DockPanel-widget, .lm-DockPanel-widget { z-index: 0; }

.p-DockPanel-tabBar, .lm-DockPanel-tabBar { z-index: 1; }

.p-DockPanel-handle, .lm-DockPanel-handle { z-index: 2; }

.p-DockPanel-handle.p-mod-hidden, .lm-DockPanel-handle.lm-mod-hidden { disp=
lay: none !important; }

.p-DockPanel-handle::after, .lm-DockPanel-handle::after { position: absolut=
e; top: 0px; left: 0px; width: 100%; height: 100%; content: ""; }

.p-DockPanel-handle[data-orientation=3D"horizontal"], .lm-DockPanel-handle[=
data-orientation=3D"horizontal"] { cursor: ew-resize; }

.p-DockPanel-handle[data-orientation=3D"vertical"], .lm-DockPanel-handle[da=
ta-orientation=3D"vertical"] { cursor: ns-resize; }

.p-DockPanel-handle[data-orientation=3D"horizontal"]::after, .lm-DockPanel-=
handle[data-orientation=3D"horizontal"]::after { left: 50%; min-width: 8px;=
 transform: translateX(-50%); }

.p-DockPanel-handle[data-orientation=3D"vertical"]::after, .lm-DockPanel-ha=
ndle[data-orientation=3D"vertical"]::after { top: 50%; min-height: 8px; tra=
nsform: translateY(-50%); }

.p-DockPanel-overlay, .lm-DockPanel-overlay { z-index: 3; box-sizing: borde=
r-box; pointer-events: none; }

.p-DockPanel-overlay.p-mod-hidden, .lm-DockPanel-overlay.lm-mod-hidden { di=
splay: none !important; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-4ba1a7b4-c904-4133-892e-2a4002beb30b@mhtml.blink

@charset "utf-8";

.p-Menu, .lm-Menu { z-index: 10000; position: absolute; white-space: nowrap=
; overflow: hidden auto; outline: none; user-select: none; }

.p-Menu-content, .lm-Menu-content { margin: 0px; padding: 0px; display: tab=
le; list-style-type: none; }

.p-Menu-item, .lm-Menu-item { display: table-row; }

.p-Menu-item.p-mod-hidden, .p-Menu-item.p-mod-collapsed, .lm-Menu-item.lm-m=
od-hidden, .lm-Menu-item.lm-mod-collapsed { display: none !important; }

.p-Menu-itemIcon, .p-Menu-itemSubmenuIcon, .lm-Menu-itemIcon, .lm-Menu-item=
SubmenuIcon { display: table-cell; text-align: center; }

.p-Menu-itemLabel, .lm-Menu-itemLabel { display: table-cell; text-align: le=
ft; }

.p-Menu-itemShortcut, .lm-Menu-itemShortcut { display: table-cell; text-ali=
gn: right; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-492c6891-d580-4652-90ff-00c3d071f793@mhtml.blink

@charset "utf-8";

.p-MenuBar, .lm-MenuBar { outline: none; user-select: none; }

.p-MenuBar-content, .lm-MenuBar-content { margin: 0px; padding: 0px; displa=
y: flex; flex-direction: row; list-style-type: none; }

.p--MenuBar-item, .lm-MenuBar-item { box-sizing: border-box; }

.p-MenuBar-itemIcon, .p-MenuBar-itemLabel, .lm-MenuBar-itemIcon, .lm-MenuBa=
r-itemLabel { display: inline-block; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-a8783c95-b9ef-4884-b3d4-b921582b750e@mhtml.blink

@charset "utf-8";

.p-ScrollBar, .lm-ScrollBar { display: flex; user-select: none; }

.p-ScrollBar[data-orientation=3D"horizontal"], .lm-ScrollBar[data-orientati=
on=3D"horizontal"] { flex-direction: row; }

.p-ScrollBar[data-orientation=3D"vertical"], .lm-ScrollBar[data-orientation=
=3D"vertical"] { flex-direction: column; }

.p-ScrollBar-button, .lm-ScrollBar-button { box-sizing: border-box; flex: 0=
 0 auto; }

.p-ScrollBar-track, .lm-ScrollBar-track { box-sizing: border-box; position:=
 relative; overflow: hidden; flex: 1 1 auto; }

.p-ScrollBar-thumb, .lm-ScrollBar-thumb { box-sizing: border-box; position:=
 absolute; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-998870eb-cf54-46b5-a917-c9493e8ba448@mhtml.blink

@charset "utf-8";

.p-SplitPanel-child, .lm-SplitPanel-child { z-index: 0; }

.p-SplitPanel-handle, .lm-SplitPanel-handle { z-index: 1; }

.p-SplitPanel-handle.p-mod-hidden, .lm-SplitPanel-handle.lm-mod-hidden { di=
splay: none !important; }

.p-SplitPanel-handle::after, .lm-SplitPanel-handle::after { position: absol=
ute; top: 0px; left: 0px; width: 100%; height: 100%; content: ""; }

.p-SplitPanel[data-orientation=3D"horizontal"] > .p-SplitPanel-handle, .lm-=
SplitPanel[data-orientation=3D"horizontal"] > .lm-SplitPanel-handle { curso=
r: ew-resize; }

.p-SplitPanel[data-orientation=3D"vertical"] > .p-SplitPanel-handle, .lm-Sp=
litPanel[data-orientation=3D"vertical"] > .lm-SplitPanel-handle { cursor: n=
s-resize; }

.p-SplitPanel[data-orientation=3D"horizontal"] > .p-SplitPanel-handle::afte=
r, .lm-SplitPanel[data-orientation=3D"horizontal"] > .lm-SplitPanel-handle:=
:after { left: 50%; min-width: 8px; transform: translateX(-50%); }

.p-SplitPanel[data-orientation=3D"vertical"] > .p-SplitPanel-handle::after,=
 .lm-SplitPanel[data-orientation=3D"vertical"] > .lm-SplitPanel-handle::aft=
er { top: 50%; min-height: 8px; transform: translateY(-50%); }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-762778e4-e802-4417-8169-e36bff4175c8@mhtml.blink

@charset "utf-8";

.p-TabBar, .lm-TabBar { display: flex; user-select: none; }

.p-TabBar[data-orientation=3D"horizontal"], .lm-TabBar[data-orientation=3D"=
horizontal"] { flex-direction: row; align-items: flex-end; }

.p-TabBar[data-orientation=3D"vertical"], .lm-TabBar[data-orientation=3D"ve=
rtical"] { flex-direction: column; align-items: flex-end; }

.p-TabBar-content, .lm-TabBar-content { margin: 0px; padding: 0px; display:=
 flex; flex: 1 1 auto; list-style-type: none; }

.p-TabBar[data-orientation=3D"horizontal"] > .p-TabBar-content, .lm-TabBar[=
data-orientation=3D"horizontal"] > .lm-TabBar-content { flex-direction: row=
; }

.p-TabBar[data-orientation=3D"vertical"] > .p-TabBar-content, .lm-TabBar[da=
ta-orientation=3D"vertical"] > .lm-TabBar-content { flex-direction: column;=
 }

.p-TabBar-tab, .lm-TabBar-tab { display: flex; flex-direction: row; box-siz=
ing: border-box; overflow: hidden; touch-action: none; }

.p-TabBar-tabIcon, .p-TabBar-tabCloseIcon, .lm-TabBar-tabIcon, .lm-TabBar-t=
abCloseIcon { flex: 0 0 auto; }

.p-TabBar-tabLabel, .lm-TabBar-tabLabel { flex: 1 1 auto; overflow: hidden;=
 white-space: nowrap; }

.lm-TabBar-tabInput { user-select: all; width: 100%; box-sizing: border-box=
; }

.p-TabBar-tab.p-mod-hidden, .lm-TabBar-tab.lm-mod-hidden { display: none !i=
mportant; }

.lm-TabBar-addButton.lm-mod-hidden { display: none !important; }

.p-TabBar.p-mod-dragging .p-TabBar-tab, .lm-TabBar.lm-mod-dragging .lm-TabB=
ar-tab { position: relative; }

.p-TabBar.p-mod-dragging[data-orientation=3D"horizontal"] .p-TabBar-tab, .l=
m-TabBar.lm-mod-dragging[data-orientation=3D"horizontal"] .lm-TabBar-tab { =
left: 0px; transition: left 150ms ease 0s; }

.p-TabBar.p-mod-dragging[data-orientation=3D"vertical"] .p-TabBar-tab, .lm-=
TabBar.lm-mod-dragging[data-orientation=3D"vertical"] .lm-TabBar-tab { top:=
 0px; transition: top 150ms ease 0s; }

.p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-dragging, .lm-TabBar.lm-mod-dr=
agging .lm-TabBar-tab.lm-mod-dragging { transition: none 0s ease 0s; }

.lm-TabBar-tabLabel .lm-TabBar-tabInput { user-select: all; width: 100%; bo=
x-sizing: border-box; background: inherit; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-35a3899a-3a68-4437-a357-187824ba8916@mhtml.blink

@charset "utf-8";

.p-TabPanel-tabBar, .lm-TabPanel-tabBar { z-index: 1; }

.p-TabPanel-stackedPanel, .lm-TabPanel-stackedPanel { z-index: 0; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-b9e99216-e19e-4d0f-941f-f0e668c88f66@mhtml.blink

@charset "utf-8";
=0A
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-22f22da9-a8a4-4cef-bd16-60fd40b7da6c@mhtml.blink

@charset "utf-8";

.jupyter-widgets-disconnected::before { content: "=EF=84=A7"; display: inli=
ne-block; font: 900 14px / 1 "Font Awesome 5 Free", FontAwesome; text-rende=
ring: auto; -webkit-font-smoothing: antialiased; color: rgb(217, 83, 79); p=
adding: 3px; align-self: flex-start; }

.jupyter-widgets-error-widget { display: flex; flex-direction: column; just=
ify-content: center; height: 100%; border: 1px solid red; margin: 0px auto;=
 }

.jupyter-widgets-error-widget.icon-error { min-width: var(--jp-widgets-inli=
ne-width-short); }

.jupyter-widgets-error-widget.text-error { min-width: calc(2 * var(--jp-wid=
gets-inline-width)); min-height: calc(3 * var(--jp-widgets-inline-height));=
 }

.jupyter-widgets-error-widget p { text-align: center; }

.jupyter-widgets-error-widget.text-error pre::first-line { font-weight: bol=
d; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-cf5c9e11-0496-4d3c-b88d-a86b837bca1d@mhtml.blink

@charset "utf-8";

:root { --md-red-50: #ffebee; --md-red-100: #ffcdd2; --md-red-200: #ef9a9a;=
 --md-red-300: #e57373; --md-red-400: #ef5350; --md-red-500: #f44336; --md-=
red-600: #e53935; --md-red-700: #d32f2f; --md-red-800: #c62828; --md-red-90=
0: #b71c1c; --md-red-A100: #ff8a80; --md-red-A200: #ff5252; --md-red-A400: =
#ff1744; --md-red-A700: #d50000; --md-pink-50: #fce4ec; --md-pink-100: #f8b=
bd0; --md-pink-200: #f48fb1; --md-pink-300: #f06292; --md-pink-400: #ec407a=
; --md-pink-500: #e91e63; --md-pink-600: #d81b60; --md-pink-700: #c2185b; -=
-md-pink-800: #ad1457; --md-pink-900: #880e4f; --md-pink-A100: #ff80ab; --m=
d-pink-A200: #ff4081; --md-pink-A400: #f50057; --md-pink-A700: #c51162; --m=
d-purple-50: #f3e5f5; --md-purple-100: #e1bee7; --md-purple-200: #ce93d8; -=
-md-purple-300: #ba68c8; --md-purple-400: #ab47bc; --md-purple-500: #9c27b0=
; --md-purple-600: #8e24aa; --md-purple-700: #7b1fa2; --md-purple-800: #6a1=
b9a; --md-purple-900: #4a148c; --md-purple-A100: #ea80fc; --md-purple-A200:=
 #e040fb; --md-purple-A400: #d500f9; --md-purple-A700: #aa00ff; --md-deep-p=
urple-50: #ede7f6; --md-deep-purple-100: #d1c4e9; --md-deep-purple-200: #b3=
9ddb; --md-deep-purple-300: #9575cd; --md-deep-purple-400: #7e57c2; --md-de=
ep-purple-500: #673ab7; --md-deep-purple-600: #5e35b1; --md-deep-purple-700=
: #512da8; --md-deep-purple-800: #4527a0; --md-deep-purple-900: #311b92; --=
md-deep-purple-A100: #b388ff; --md-deep-purple-A200: #7c4dff; --md-deep-pur=
ple-A400: #651fff; --md-deep-purple-A700: #6200ea; --md-indigo-50: #e8eaf6;=
 --md-indigo-100: #c5cae9; --md-indigo-200: #9fa8da; --md-indigo-300: #7986=
cb; --md-indigo-400: #5c6bc0; --md-indigo-500: #3f51b5; --md-indigo-600: #3=
949ab; --md-indigo-700: #303f9f; --md-indigo-800: #283593; --md-indigo-900:=
 #1a237e; --md-indigo-A100: #8c9eff; --md-indigo-A200: #536dfe; --md-indigo=
-A400: #3d5afe; --md-indigo-A700: #304ffe; --md-blue-50: #e3f2fd; --md-blue=
-100: #bbdefb; --md-blue-200: #90caf9; --md-blue-300: #64b5f6; --md-blue-40=
0: #42a5f5; --md-blue-500: #2196f3; --md-blue-600: #1e88e5; --md-blue-700: =
#1976d2; --md-blue-800: #1565c0; --md-blue-900: #0d47a1; --md-blue-A100: #8=
2b1ff; --md-blue-A200: #448aff; --md-blue-A400: #2979ff; --md-blue-A700: #2=
962ff; --md-light-blue-50: #e1f5fe; --md-light-blue-100: #b3e5fc; --md-ligh=
t-blue-200: #81d4fa; --md-light-blue-300: #4fc3f7; --md-light-blue-400: #29=
b6f6; --md-light-blue-500: #03a9f4; --md-light-blue-600: #039be5; --md-ligh=
t-blue-700: #0288d1; --md-light-blue-800: #0277bd; --md-light-blue-900: #01=
579b; --md-light-blue-A100: #80d8ff; --md-light-blue-A200: #40c4ff; --md-li=
ght-blue-A400: #00b0ff; --md-light-blue-A700: #0091ea; --md-cyan-50: #e0f7f=
a; --md-cyan-100: #b2ebf2; --md-cyan-200: #80deea; --md-cyan-300: #4dd0e1; =
--md-cyan-400: #26c6da; --md-cyan-500: #00bcd4; --md-cyan-600: #00acc1; --m=
d-cyan-700: #0097a7; --md-cyan-800: #00838f; --md-cyan-900: #006064; --md-c=
yan-A100: #84ffff; --md-cyan-A200: #18ffff; --md-cyan-A400: #00e5ff; --md-c=
yan-A700: #00b8d4; --md-teal-50: #e0f2f1; --md-teal-100: #b2dfdb; --md-teal=
-200: #80cbc4; --md-teal-300: #4db6ac; --md-teal-400: #26a69a; --md-teal-50=
0: #009688; --md-teal-600: #00897b; --md-teal-700: #00796b; --md-teal-800: =
#00695c; --md-teal-900: #004d40; --md-teal-A100: #a7ffeb; --md-teal-A200: #=
64ffda; --md-teal-A400: #1de9b6; --md-teal-A700: #00bfa5; --md-green-50: #e=
8f5e9; --md-green-100: #c8e6c9; --md-green-200: #a5d6a7; --md-green-300: #8=
1c784; --md-green-400: #66bb6a; --md-green-500: #4caf50; --md-green-600: #4=
3a047; --md-green-700: #388e3c; --md-green-800: #2e7d32; --md-green-900: #1=
b5e20; --md-green-A100: #b9f6ca; --md-green-A200: #69f0ae; --md-green-A400:=
 #00e676; --md-green-A700: #00c853; --md-light-green-50: #f1f8e9; --md-ligh=
t-green-100: #dcedc8; --md-light-green-200: #c5e1a5; --md-light-green-300: =
#aed581; --md-light-green-400: #9ccc65; --md-light-green-500: #8bc34a; --md=
-light-green-600: #7cb342; --md-light-green-700: #689f38; --md-light-green-=
800: #558b2f; --md-light-green-900: #33691e; --md-light-green-A100: #ccff90=
; --md-light-green-A200: #b2ff59; --md-light-green-A400: #76ff03; --md-ligh=
t-green-A700: #64dd17; --md-lime-50: #f9fbe7; --md-lime-100: #f0f4c3; --md-=
lime-200: #e6ee9c; --md-lime-300: #dce775; --md-lime-400: #d4e157; --md-lim=
e-500: #cddc39; --md-lime-600: #c0ca33; --md-lime-700: #afb42b; --md-lime-8=
00: #9e9d24; --md-lime-900: #827717; --md-lime-A100: #f4ff81; --md-lime-A20=
0: #eeff41; --md-lime-A400: #c6ff00; --md-lime-A700: #aeea00; --md-yellow-5=
0: #fffde7; --md-yellow-100: #fff9c4; --md-yellow-200: #fff59d; --md-yellow=
-300: #fff176; --md-yellow-400: #ffee58; --md-yellow-500: #ffeb3b; --md-yel=
low-600: #fdd835; --md-yellow-700: #fbc02d; --md-yellow-800: #f9a825; --md-=
yellow-900: #f57f17; --md-yellow-A100: #ffff8d; --md-yellow-A200: #ffff00; =
--md-yellow-A400: #ffea00; --md-yellow-A700: #ffd600; --md-amber-50: #fff8e=
1; --md-amber-100: #ffecb3; --md-amber-200: #ffe082; --md-amber-300: #ffd54=
f; --md-amber-400: #ffca28; --md-amber-500: #ffc107; --md-amber-600: #ffb30=
0; --md-amber-700: #ffa000; --md-amber-800: #ff8f00; --md-amber-900: #ff6f0=
0; --md-amber-A100: #ffe57f; --md-amber-A200: #ffd740; --md-amber-A400: #ff=
c400; --md-amber-A700: #ffab00; --md-orange-50: #fff3e0; --md-orange-100: #=
ffe0b2; --md-orange-200: #ffcc80; --md-orange-300: #ffb74d; --md-orange-400=
: #ffa726; --md-orange-500: #ff9800; --md-orange-600: #fb8c00; --md-orange-=
700: #f57c00; --md-orange-800: #ef6c00; --md-orange-900: #e65100; --md-oran=
ge-A100: #ffd180; --md-orange-A200: #ffab40; --md-orange-A400: #ff9100; --m=
d-orange-A700: #ff6d00; --md-deep-orange-50: #fbe9e7; --md-deep-orange-100:=
 #ffccbc; --md-deep-orange-200: #ffab91; --md-deep-orange-300: #ff8a65; --m=
d-deep-orange-400: #ff7043; --md-deep-orange-500: #ff5722; --md-deep-orange=
-600: #f4511e; --md-deep-orange-700: #e64a19; --md-deep-orange-800: #d84315=
; --md-deep-orange-900: #bf360c; --md-deep-orange-A100: #ff9e80; --md-deep-=
orange-A200: #ff6e40; --md-deep-orange-A400: #ff3d00; --md-deep-orange-A700=
: #dd2c00; --md-brown-50: #efebe9; --md-brown-100: #d7ccc8; --md-brown-200:=
 #bcaaa4; --md-brown-300: #a1887f; --md-brown-400: #8d6e63; --md-brown-500:=
 #795548; --md-brown-600: #6d4c41; --md-brown-700: #5d4037; --md-brown-800:=
 #4e342e; --md-brown-900: #3e2723; --md-grey-50: #fafafa; --md-grey-100: #f=
5f5f5; --md-grey-200: #eeeeee; --md-grey-300: #e0e0e0; --md-grey-400: #bdbd=
bd; --md-grey-500: #9e9e9e; --md-grey-600: #757575; --md-grey-700: #616161;=
 --md-grey-800: #424242; --md-grey-900: #212121; --md-blue-grey-50: #eceff1=
; --md-blue-grey-100: #cfd8dc; --md-blue-grey-200: #b0bec5; --md-blue-grey-=
300: #90a4ae; --md-blue-grey-400: #78909c; --md-blue-grey-500: #607d8b; --m=
d-blue-grey-600: #546e7a; --md-blue-grey-700: #455a64; --md-blue-grey-800: =
#37474f; --md-blue-grey-900: #263238; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-cbc856b7-4060-4ee6-97c7-f0fed95caf41@mhtml.blink

@charset "utf-8";

:root { --jp-icon-search: none; --jp-ui-select-caret: none; }

:root { --jp-border-width: 1px; --jp-border-color0: var(--md-grey-700); --j=
p-border-color1: var(--md-grey-500); --jp-border-color2: var(--md-grey-300)=
; --jp-border-color3: var(--md-grey-100); --jp-ui-icon-font-size: 14px; --j=
p-ui-font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; --jp-ui-f=
ont-color0: rgba(0, 0, 0, 1); --jp-ui-font-color1: rgba(0, 0, 0, 0.8); --jp=
-ui-font-color2: rgba(0, 0, 0, 0.5); --jp-ui-font-color3: rgba(0, 0, 0, 0.3=
); --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1); --jp-ui-inverse-fon=
t-color1: rgba(255, 255, 255, 1); --jp-ui-inverse-font-color2: rgba(255, 25=
5, 255, 0.7); --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5); --jp-c=
ontent-font-size: 13px; --jp-content-line-height: 1.5; --jp-content-font-co=
lor0: black; --jp-content-font-color1: black; --jp-content-font-color2: var=
(--md-grey-700); --jp-content-font-color3: var(--md-grey-500); --jp-ui-font=
-scale-factor: 1.2; --jp-ui-font-size0: calc(
    var(--jp-ui-font-size1) / var(--jp-ui-font-scale-factor)
  ); --jp-ui-font-size1: 13px; --jp-ui-font-size2: calc(
    var(--jp-ui-font-size1) * var(--jp-ui-font-scale-factor)
  ); --jp-ui-font-size3: calc(
    var(--jp-ui-font-size2) * var(--jp-ui-font-scale-factor)
  ); --jp-code-font-size: 13px; --jp-code-line-height: 1.307; --jp-code-pad=
ding: 5px; --jp-code-font-family: monospace; --jp-layout-color0: white; --j=
p-layout-color1: white; --jp-layout-color2: var(--md-grey-200); --jp-layout=
-color3: var(--md-grey-400); --jp-brand-color0: var(--md-blue-700); --jp-br=
and-color1: var(--md-blue-500); --jp-brand-color2: var(--md-blue-300); --jp=
-brand-color3: var(--md-blue-100); --jp-accent-color0: var(--md-green-700);=
 --jp-accent-color1: var(--md-green-500); --jp-accent-color2: var(--md-gree=
n-300); --jp-accent-color3: var(--md-green-100); --jp-warn-color0: var(--md=
-orange-700); --jp-warn-color1: var(--md-orange-500); --jp-warn-color2: var=
(--md-orange-300); --jp-warn-color3: var(--md-orange-100); --jp-error-color=
0: var(--md-red-700); --jp-error-color1: var(--md-red-500); --jp-error-colo=
r2: var(--md-red-300); --jp-error-color3: var(--md-red-100); --jp-success-c=
olor0: var(--md-green-700); --jp-success-color1: var(--md-green-500); --jp-=
success-color2: var(--md-green-300); --jp-success-color3: var(--md-green-10=
0); --jp-info-color0: var(--md-cyan-700); --jp-info-color1: var(--md-cyan-5=
00); --jp-info-color2: var(--md-cyan-300); --jp-info-color3: var(--md-cyan-=
100); --jp-cell-padding: 5px; --jp-cell-editor-background: #f7f7f7; --jp-ce=
ll-editor-border-color: #cfcfcf; --jp-cell-editor-background-edit: var(--jp=
-ui-layout-color1); --jp-cell-editor-border-color-edit: var(--jp-brand-colo=
r1); --jp-cell-prompt-width: 100px; --jp-cell-prompt-font-family: 'Roboto M=
ono', monospace; --jp-cell-prompt-letter-spacing: 0px; --jp-cell-prompt-opa=
city: 1; --jp-cell-prompt-opacity-not-active: 0.4; --jp-cell-prompt-font-co=
lor-not-active: var(--md-grey-700); --jp-cell-inprompt-font-color: #307fc1;=
 --jp-cell-outprompt-font-color: #bf5b3d; --jp-notebook-padding: 10px; --jp=
-notebook-scroll-padding: 100px; --jp-console-background: var(--md-grey-100=
); --jp-toolbar-border-color: var(--md-grey-400); --jp-toolbar-micro-height=
: 8px; --jp-toolbar-background: var(--jp-layout-color0); --jp-toolbar-box-s=
hadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24); --jp-toolbar-header-margin: 4px=
 4px 0px 4px; --jp-toolbar-active-background: var(--md-grey-300); }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-ae5dcdd6-9045-4819-b495-d9566b7acc94@mhtml.blink

@charset "utf-8";

.jupyter-widgets.widget-tab > .p-TabBar, .jupyter-widgets.jupyter-widget-ta=
b > .p-TabBar, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar { display: =
flex; user-select: none; }

.jupyter-widgets.widget-tab > .p-TabBar[data-orientation=3D"horizontal"], .=
jupyter-widgets.jupyter-widget-tab > .p-TabBar[data-orientation=3D"horizont=
al"], .jupyter-widgets.jupyter-widget-tab > .lm-TabBar[data-orientation=3D"=
horizontal"] { flex-direction: row; }

.jupyter-widgets.widget-tab > .p-TabBar[data-orientation=3D"vertical"], .ju=
pyter-widgets.jupyter-widget-tab > .p-TabBar[data-orientation=3D"vertical"]=
, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar[data-orientation=3D"vert=
ical"] { flex-direction: column; }

.jupyter-widgets.widget-tab > .p-TabBar > .p-TabBar-content, .jupyter-widge=
ts.jupyter-widget-tab > .p-TabBar > .p-TabBar-content, .jupyter-widgets.jup=
yter-widget-tab > .lm-TabBar > .lm-TabBar-content { margin: 0px; padding: 0=
px; display: flex; flex: 1 1 auto; list-style-type: none; }

.jupyter-widgets.widget-tab > .p-TabBar[data-orientation=3D"horizontal"] > =
.p-TabBar-content, .jupyter-widgets.jupyter-widget-tab > .p-TabBar[data-ori=
entation=3D"horizontal"] > .p-TabBar-content, .jupyter-widgets.jupyter-widg=
et-tab > .lm-TabBar[data-orientation=3D"horizontal"] > .lm-TabBar-content {=
 flex-direction: row; }

.jupyter-widgets.widget-tab > .p-TabBar[data-orientation=3D"vertical"] > .p=
-TabBar-content, .jupyter-widgets.jupyter-widget-tab > .p-TabBar[data-orien=
tation=3D"vertical"] > .p-TabBar-content, .jupyter-widgets.jupyter-widget-t=
ab > .lm-TabBar[data-orientation=3D"vertical"] > .lm-TabBar-content { flex-=
direction: column; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab, .jupyter-widgets.jup=
yter-widget-tab > .p-TabBar .p-TabBar-tab, .jupyter-widgets.jupyter-widget-=
tab > .lm-TabBar .lm-TabBar-tab { display: flex; flex-direction: row; box-s=
izing: border-box; overflow: hidden; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tabIcon, .jupyter-widgets=
.widget-tab > .p-TabBar .p-TabBar-tabCloseIcon, .jupyter-widgets.jupyter-wi=
dget-tab > .p-TabBar .p-TabBar-tabIcon, .jupyter-widgets.jupyter-widget-tab=
 > .p-TabBar .p-TabBar-tabCloseIcon, .jupyter-widgets.jupyter-widget-tab > =
.lm-TabBar .lm-TabBar-tabIcon, .jupyter-widgets.jupyter-widget-tab > .lm-Ta=
bBar .lm-TabBar-tabCloseIcon { flex: 0 0 auto; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tabLabel, .jupyter-widget=
s.jupyter-widget-tab > .p-TabBar .p-TabBar-tabLabel, .jupyter-widgets.jupyt=
er-widget-tab > .lm-TabBar .lm-TabBar-tabLabel { flex: 1 1 auto; overflow: =
hidden; white-space: nowrap; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab.p-mod-hidden, .jupyte=
r-widgets.jupyter-widget-tab > .p-TabBar .p-TabBar-tab.p-mod-hidden, .jupyt=
er-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-tab.lm-mod-hidden { d=
isplay: none !important; }

.jupyter-widgets.widget-tab > .p-TabBar.p-mod-dragging .p-TabBar-tab, .jupy=
ter-widgets.jupyter-widget-tab > .p-TabBar.p-mod-dragging .p-TabBar-tab, .j=
upyter-widgets.jupyter-widget-tab > .lm-TabBar.lm-mod-dragging .lm-TabBar-t=
ab { position: relative; }

.jupyter-widgets.widget-tab > .p-TabBar.p-mod-dragging[data-orientation=3D"=
horizontal"] .p-TabBar-tab, .jupyter-widgets.jupyter-widget-tab > .p-TabBar=
.p-mod-dragging[data-orientation=3D"horizontal"] .p-TabBar-tab, .jupyter-wi=
dgets.jupyter-widget-tab > .lm-TabBar.lm-mod-dragging[data-orientation=3D"h=
orizontal"] .lm-TabBar-tab { left: 0px; transition: left 150ms ease 0s; }

.jupyter-widgets.widget-tab > .p-TabBar.p-mod-dragging[data-orientation=3D"=
vertical"] .p-TabBar-tab, .jupyter-widgets.jupyter-widget-tab > .p-TabBar.p=
-mod-dragging[data-orientation=3D"vertical"] .p-TabBar-tab, .jupyter-widget=
s.jupyter-widget-tab > .lm-TabBar.lm-mod-dragging[data-orientation=3D"verti=
cal"] .lm-TabBar-tab { top: 0px; transition: top 150ms ease 0s; }

.jupyter-widgets.widget-tab > .p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-=
dragging, .jupyter-widgets.jupyter-widget-tab > .p-TabBar.p-mod-dragging .p=
-TabBar-tab.p-mod-dragging, .jupyter-widgets.jupyter-widget-tab > .lm-TabBa=
r.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging { transition: none 0s ease=
 0s; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-e5247429-5cc2-4e23-bd91-8acda443531f@mhtml.blink

@charset "utf-8";

.widget-slider, .jupyter-widget-slider { }

.widget-slider .noUi-target, .jupyter-widget-slider .noUi-target, .widget-s=
lider .noUi-target *, .jupyter-widget-slider .noUi-target * { -webkit-tap-h=
ighlight-color: rgba(0, 0, 0, 0); touch-action: none; user-select: none; bo=
x-sizing: border-box; }

.widget-slider .noUi-target, .jupyter-widget-slider .noUi-target { position=
: relative; }

.widget-slider .noUi-base, .jupyter-widget-slider .noUi-base, .widget-slide=
r .noUi-connects, .jupyter-widget-slider .noUi-connects { width: 100%; heig=
ht: 100%; position: relative; z-index: 1; }

.widget-slider .noUi-connects, .jupyter-widget-slider .noUi-connects { over=
flow: hidden; z-index: 0; }

.widget-slider .noUi-connect, .jupyter-widget-slider .noUi-connect, .widget=
-slider .noUi-origin, .jupyter-widget-slider .noUi-origin { will-change: tr=
ansform; position: absolute; z-index: 1; top: 0px; right: 0px; transform-or=
igin: 0px 0px; transform-style: flat; }

.widget-slider .noUi-connect, .jupyter-widget-slider .noUi-connect { height=
: 100%; width: 100%; }

.widget-slider .noUi-origin, .jupyter-widget-slider .noUi-origin { height: =
10%; width: 10%; }

.widget-slider .noUi-txt-dir-rtl.noUi-horizontal .noUi-origin, .jupyter-wid=
get-slider .noUi-txt-dir-rtl.noUi-horizontal .noUi-origin { left: 0px; righ=
t: auto; }

.widget-slider .noUi-vertical .noUi-origin, .jupyter-widget-slider .noUi-ve=
rtical .noUi-origin { width: 0px; }

.widget-slider .noUi-horizontal .noUi-origin, .jupyter-widget-slider .noUi-=
horizontal .noUi-origin { height: 0px; }

.widget-slider .noUi-handle, .jupyter-widget-slider .noUi-handle { backface=
-visibility: hidden; position: absolute; }

.widget-slider .noUi-touch-area, .jupyter-widget-slider .noUi-touch-area { =
height: 100%; width: 100%; }

.widget-slider .noUi-state-tap .noUi-connect, .jupyter-widget-slider .noUi-=
state-tap .noUi-connect, .widget-slider .noUi-state-tap .noUi-origin, .jupy=
ter-widget-slider .noUi-state-tap .noUi-origin { transition: transform 0.3s=
 ease 0s; }

.widget-slider .noUi-state-drag *, .jupyter-widget-slider .noUi-state-drag =
* { cursor: inherit !important; }

.widget-slider .noUi-horizontal, .jupyter-widget-slider .noUi-horizontal { =
height: 18px; }

.widget-slider .noUi-horizontal .noUi-handle, .jupyter-widget-slider .noUi-=
horizontal .noUi-handle { width: 34px; height: 28px; right: -17px; top: -6p=
x; }

.widget-slider .noUi-vertical, .jupyter-widget-slider .noUi-vertical { widt=
h: 18px; }

.widget-slider .noUi-vertical .noUi-handle, .jupyter-widget-slider .noUi-ve=
rtical .noUi-handle { width: 28px; height: 34px; right: -6px; top: -17px; }

.widget-slider .noUi-txt-dir-rtl.noUi-horizontal .noUi-handle, .jupyter-wid=
get-slider .noUi-txt-dir-rtl.noUi-horizontal .noUi-handle { left: -17px; ri=
ght: auto; }

.widget-slider .noUi-target, .jupyter-widget-slider .noUi-target { backgrou=
nd: rgb(250, 250, 250); border-radius: 4px; border: 1px solid rgb(211, 211,=
 211); box-shadow: rgb(240, 240, 240) 0px 1px 1px inset, rgb(187, 187, 187)=
 0px 3px 6px -5px; }

.widget-slider .noUi-connects, .jupyter-widget-slider .noUi-connects { bord=
er-radius: 3px; }

.widget-slider .noUi-connect, .jupyter-widget-slider .noUi-connect { backgr=
ound: rgb(63, 184, 175); }

.widget-slider .noUi-draggable, .jupyter-widget-slider .noUi-draggable { cu=
rsor: ew-resize; }

.widget-slider .noUi-vertical .noUi-draggable, .jupyter-widget-slider .noUi=
-vertical .noUi-draggable { cursor: ns-resize; }

.widget-slider .noUi-handle, .jupyter-widget-slider .noUi-handle { border: =
1px solid rgb(217, 217, 217); border-radius: 3px; background: rgb(255, 255,=
 255); cursor: default; box-shadow: rgb(255, 255, 255) 0px 0px 1px inset, r=
gb(235, 235, 235) 0px 1px 7px inset, rgb(187, 187, 187) 0px 3px 6px -3px; }

.widget-slider .noUi-active, .jupyter-widget-slider .noUi-active { box-shad=
ow: rgb(255, 255, 255) 0px 0px 1px inset, rgb(221, 221, 221) 0px 1px 7px in=
set, rgb(187, 187, 187) 0px 3px 6px -3px; }

.widget-slider .noUi-handle::before, .jupyter-widget-slider .noUi-handle::b=
efore, .widget-slider .noUi-handle::after, .jupyter-widget-slider .noUi-han=
dle::after { content: ""; display: block; position: absolute; height: 14px;=
 width: 1px; background: rgb(232, 231, 230); left: 14px; top: 6px; }

.widget-slider .noUi-handle::after, .jupyter-widget-slider .noUi-handle::af=
ter { left: 17px; }

.widget-slider .noUi-vertical .noUi-handle::before, .jupyter-widget-slider =
.noUi-vertical .noUi-handle::before, .widget-slider .noUi-vertical .noUi-ha=
ndle::after, .jupyter-widget-slider .noUi-vertical .noUi-handle::after { wi=
dth: 14px; height: 1px; left: 6px; top: 14px; }

.widget-slider .noUi-vertical .noUi-handle::after, .jupyter-widget-slider .=
noUi-vertical .noUi-handle::after { top: 17px; }

.widget-slider [disabled] .noUi-connect, .jupyter-widget-slider [disabled] =
.noUi-connect { background: rgb(184, 184, 184); }

.widget-slider [disabled].noUi-target, .jupyter-widget-slider [disabled].no=
Ui-target, .widget-slider [disabled].noUi-handle, .jupyter-widget-slider [d=
isabled].noUi-handle, .widget-slider [disabled] .noUi-handle, .jupyter-widg=
et-slider [disabled] .noUi-handle { cursor: not-allowed; }

.widget-slider .noUi-pips, .jupyter-widget-slider .noUi-pips, .widget-slide=
r .noUi-pips *, .jupyter-widget-slider .noUi-pips * { box-sizing: border-bo=
x; }

.widget-slider .noUi-pips, .jupyter-widget-slider .noUi-pips { position: ab=
solute; color: rgb(153, 153, 153); }

.widget-slider .noUi-value, .jupyter-widget-slider .noUi-value { position: =
absolute; white-space: nowrap; text-align: center; }

.widget-slider .noUi-value-sub, .jupyter-widget-slider .noUi-value-sub { co=
lor: rgb(204, 204, 204); font-size: 10px; }

.widget-slider .noUi-marker, .jupyter-widget-slider .noUi-marker { position=
: absolute; background: rgb(204, 204, 204); }

.widget-slider .noUi-marker-sub, .jupyter-widget-slider .noUi-marker-sub { =
background: rgb(170, 170, 170); }

.widget-slider .noUi-marker-large, .jupyter-widget-slider .noUi-marker-larg=
e { background: rgb(170, 170, 170); }

.widget-slider .noUi-pips-horizontal, .jupyter-widget-slider .noUi-pips-hor=
izontal { padding: 10px 0px; height: 80px; top: 100%; left: 0px; width: 100=
%; }

.widget-slider .noUi-value-horizontal, .jupyter-widget-slider .noUi-value-h=
orizontal { transform: translate(-50%, 50%); }

.noUi-rtl .widget-slider .noUi-value-horizontal, .noUi-rtl .jupyter-widget-=
slider .noUi-value-horizontal { transform: translate(50%, 50%); }

.widget-slider .noUi-marker-horizontal.noUi-marker, .jupyter-widget-slider =
.noUi-marker-horizontal.noUi-marker { margin-left: -1px; width: 2px; height=
: 5px; }

.widget-slider .noUi-marker-horizontal.noUi-marker-sub, .jupyter-widget-sli=
der .noUi-marker-horizontal.noUi-marker-sub { height: 10px; }

.widget-slider .noUi-marker-horizontal.noUi-marker-large, .jupyter-widget-s=
lider .noUi-marker-horizontal.noUi-marker-large { height: 15px; }

.widget-slider .noUi-pips-vertical, .jupyter-widget-slider .noUi-pips-verti=
cal { padding: 0px 10px; height: 100%; top: 0px; left: 100%; }

.widget-slider .noUi-value-vertical, .jupyter-widget-slider .noUi-value-ver=
tical { transform: translate(0px, -50%); padding-left: 25px; }

.noUi-rtl .widget-slider .noUi-value-vertical, .noUi-rtl .jupyter-widget-sl=
ider .noUi-value-vertical { transform: translate(0px, 50%); }

.widget-slider .noUi-marker-vertical.noUi-marker, .jupyter-widget-slider .n=
oUi-marker-vertical.noUi-marker { width: 5px; height: 2px; margin-top: -1px=
; }

.widget-slider .noUi-marker-vertical.noUi-marker-sub, .jupyter-widget-slide=
r .noUi-marker-vertical.noUi-marker-sub { width: 10px; }

.widget-slider .noUi-marker-vertical.noUi-marker-large, .jupyter-widget-sli=
der .noUi-marker-vertical.noUi-marker-large { width: 15px; }

.widget-slider .noUi-tooltip, .jupyter-widget-slider .noUi-tooltip { displa=
y: block; position: absolute; border: 1px solid rgb(217, 217, 217); border-=
radius: 3px; background: rgb(255, 255, 255); color: rgb(0, 0, 0); padding: =
5px; text-align: center; white-space: nowrap; }

.widget-slider .noUi-horizontal .noUi-tooltip, .jupyter-widget-slider .noUi=
-horizontal .noUi-tooltip { transform: translate(-50%, 0px); left: 50%; bot=
tom: 120%; }

.widget-slider .noUi-vertical .noUi-tooltip, .jupyter-widget-slider .noUi-v=
ertical .noUi-tooltip { transform: translate(0px, -50%); top: 50%; right: 1=
20%; }

.widget-slider .noUi-horizontal .noUi-origin > .noUi-tooltip, .jupyter-widg=
et-slider .noUi-horizontal .noUi-origin > .noUi-tooltip { transform: transl=
ate(50%, 0px); left: auto; bottom: 10px; }

.widget-slider .noUi-vertical .noUi-origin > .noUi-tooltip, .jupyter-widget=
-slider .noUi-vertical .noUi-origin > .noUi-tooltip { transform: translate(=
0px, -18px); top: auto; right: 28px; }

.widget-slider .noUi-connect, .jupyter-widget-slider .noUi-connect { backgr=
ound: rgb(33, 150, 243); }

.widget-slider .noUi-horizontal, .jupyter-widget-slider .noUi-horizontal { =
height: var(--jp-widgets-slider-track-thickness); }

.widget-slider .noUi-vertical, .jupyter-widget-slider .noUi-vertical { widt=
h: var(--jp-widgets-slider-track-thickness); height: 100%; }

.widget-slider .noUi-horizontal .noUi-handle, .jupyter-widget-slider .noUi-=
horizontal .noUi-handle { width: var(--jp-widgets-slider-handle-size); heig=
ht: var(--jp-widgets-slider-handle-size); border-radius: 50%; top: calc((va=
r(--jp-widgets-slider-track-thickness) - var(--jp-widgets-slider-handle-siz=
e)) / 2); right: calc(var(--jp-widgets-slider-handle-size) / -2); }

.widget-slider .noUi-vertical .noUi-handle, .jupyter-widget-slider .noUi-ve=
rtical .noUi-handle { height: var(--jp-widgets-slider-handle-size); width: =
var(--jp-widgets-slider-handle-size); border-radius: 50%; right: calc((var(=
--jp-widgets-slider-handle-size) - var(--jp-widgets-slider-track-thickness)=
) / -2); top: calc(var(--jp-widgets-slider-handle-size) / -2); }

.widget-slider .noUi-handle::after, .jupyter-widget-slider .noUi-handle::af=
ter { content: none; }

.widget-slider .noUi-handle::before, .jupyter-widget-slider .noUi-handle::b=
efore { content: none; }

.widget-slider .noUi-target, .jupyter-widget-slider .noUi-target { backgrou=
nd: rgb(250, 250, 250); border-radius: 4px; border: 1px; }

.widget-slider .ui-slider, .jupyter-widget-slider .ui-slider { border: var(=
--jp-widgets-slider-border-width) solid var(--jp-layout-color3); background=
: var(--jp-layout-color3); box-sizing: border-box; position: relative; bord=
er-radius: 0px; }

.widget-slider .noUi-handle, .jupyter-widget-slider .noUi-handle { width: v=
ar(--jp-widgets-slider-handle-size); border: 1px solid rgb(217, 217, 217); =
border-radius: 3px; background: rgb(255, 255, 255); cursor: default; box-sh=
adow: none; outline: none; }

.widget-slider .noUi-target:not([disabled]) .noUi-handle:hover, .jupyter-wi=
dget-slider .noUi-target:not([disabled]) .noUi-handle:hover, .widget-slider=
 .noUi-target:not([disabled]) .noUi-handle:focus, .jupyter-widget-slider .n=
oUi-target:not([disabled]) .noUi-handle:focus { background-color: var(--jp-=
widgets-slider-active-handle-color); border: var(--jp-widgets-slider-border=
-width) solid var(--jp-widgets-slider-active-handle-color); }

.widget-slider [disabled].noUi-target, .jupyter-widget-slider [disabled].no=
Ui-target { opacity: 0.35; }

.widget-slider .noUi-connects, .jupyter-widget-slider .noUi-connects { over=
flow: visible; z-index: 0; background: var(--jp-layout-color3); }

.widget-slider .noUi-vertical .noUi-connect, .jupyter-widget-slider .noUi-v=
ertical .noUi-connect { width: calc(100% + 2px); right: -1px; }

.widget-slider .noUi-horizontal .noUi-connect, .jupyter-widget-slider .noUi=
-horizontal .noUi-connect { height: calc(100% + 2px); top: -1px; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-032bdaa1-972d-4a50-8866-40e7a05b517c@mhtml.blink

@charset "utf-8";

:root { --jp-widgets-color: var(--jp-content-font-color1); --jp-widgets-lab=
el-color: var(--jp-widgets-color); --jp-widgets-readout-color: var(--jp-wid=
gets-color); --jp-widgets-font-size: var(--jp-ui-font-size1); --jp-widgets-=
margin: 2px; --jp-widgets-inline-height: 28px; --jp-widgets-inline-width: 3=
00px; --jp-widgets-inline-width-short: calc(
    var(--jp-widgets-inline-width) / 2 - var(--jp-widgets-margin)
  ); --jp-widgets-inline-width-tiny: calc(
    var(--jp-widgets-inline-width-short) / 2 - var(--jp-widgets-margin)
  ); --jp-widgets-inline-margin: 4px; --jp-widgets-inline-label-width: 80px=
; --jp-widgets-border-width: var(--jp-border-width); --jp-widgets-vertical-=
height: 200px; --jp-widgets-horizontal-tab-height: 24px; --jp-widgets-horiz=
ontal-tab-width: 144px; --jp-widgets-horizontal-tab-top-border: 2px; --jp-w=
idgets-progress-thickness: 20px; --jp-widgets-container-padding: 15px; --jp=
-widgets-input-padding: 4px; --jp-widgets-radio-item-height-adjustment: 8px=
; --jp-widgets-radio-item-height: calc(
    var(--jp-widgets-inline-height) -
      var(--jp-widgets-radio-item-height-adjustment)
  ); --jp-widgets-slider-track-thickness: 4px; --jp-widgets-slider-border-w=
idth: var(--jp-widgets-border-width); --jp-widgets-slider-handle-size: 16px=
; --jp-widgets-slider-handle-border-color: var(--jp-border-color1); --jp-wi=
dgets-slider-handle-background-color: var(--jp-layout-color1); --jp-widgets=
-slider-active-handle-color: var(--jp-brand-color1); --jp-widgets-menu-item=
-height: 24px; --jp-widgets-dropdown-arrow: url(data:image/svg+xml;base64,P=
D94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4KPCEtLSBHZW5lcmF0b3I6IEFk=
b2JlIElsbHVzdHJhdG9yIDE5LjIuMSwgU1ZHIEV4cG9ydCBQbHVnLUluIC4gU1ZHIFZlcnNpb24=
6IDYuMDAgQnVpbGQgMCkgIC0tPgo8c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG=
5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cud=
zMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IgoJIHZpZXdCb3g9IjAgMCAxOCAxOCIg=
c3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgMTggMTg7IiB4bWw6c3BhY2U9InByZXN=
lcnZlIj4KPHN0eWxlIHR5cGU9InRleHQvY3NzIj4KCS5zdDB7ZmlsbDpub25lO30KPC9zdHlsZT=
4KPHBhdGggZD0iTTUuMiw1LjlMOSw5LjdsMy44LTMuOGwxLjIsMS4ybC00LjksNWwtNC45LTVMN=
S4yLDUuOXoiLz4KPHBhdGggY2xhc3M9InN0MCIgZD0iTTAtMC42aDE4djE4SDBWLTAuNnoiLz4K=
PC9zdmc+Cg); --jp-widgets-input-color: var(--jp-ui-font-color1); --jp-widge=
ts-input-background-color: var(--jp-layout-color1); --jp-widgets-input-bord=
er-color: var(--jp-border-color1); --jp-widgets-input-focus-border-color: v=
ar(--jp-brand-color2); --jp-widgets-input-border-width: var(--jp-widgets-bo=
rder-width); --jp-widgets-disabled-opacity: 0.6; --md-shadow-key-umbra-opac=
ity: 0.2; --md-shadow-key-penumbra-opacity: 0.14; --md-shadow-ambient-shado=
w-opacity: 0.12; }

.jupyter-widgets { margin: var(--jp-widgets-margin); box-sizing: border-box=
; color: var(--jp-widgets-color); overflow: visible; }

.jp-Output-result > .jupyter-widgets { margin-left: 0px; margin-right: 0px;=
 }

.widget-inline-hbox, .jupyter-widget-inline-hbox { box-sizing: border-box; =
display: flex; flex-direction: row; align-items: baseline; }

.widget-inline-vbox, .jupyter-widget-inline-vbox { box-sizing: border-box; =
display: flex; flex-direction: column; align-items: center; }

.widget-box, .jupyter-widget-box { box-sizing: border-box; display: flex; m=
argin: 0px; overflow: auto; }

.widget-gridbox, .jupyter-widget-gridbox { box-sizing: border-box; display:=
 grid; margin: 0px; overflow: auto; }

.widget-hbox, .jupyter-widget-hbox { flex-direction: row; }

.widget-vbox, .jupyter-widget-vbox { flex-direction: column; }

.jupyter-widget-tagsinput { display: flex; flex-flow: wrap; align-items: ce=
nter; overflow: auto; cursor: text; }

.jupyter-widget-tag { padding: 0px 10px; display: inline-block; white-space=
: nowrap; overflow: hidden; text-overflow: ellipsis; text-align: center; fo=
nt-size: var(--jp-widgets-font-size); height: calc(var(--jp-widgets-inline-=
height) - 2px); line-height: calc(var(--jp-widgets-inline-height) - 2px); b=
ox-shadow: none; color: var(--jp-ui-font-color1); background-color: var(--j=
p-layout-color2); border: none; user-select: none; cursor: grab; transition=
: margin-left 200ms ease 0s; margin: 1px; }

.jupyter-widget-tag.mod-active { box-shadow: 0 4px 5px 0 rgba(0, 0, 0, var(=
--md-shadow-key-penumbra-opacity)),
    0 1px 10px 0 rgba(0, 0, 0, var(--md-shadow-ambient-shadow-opacity)),
    0 2px 4px -1px rgba(0, 0, 0, var(--md-shadow-key-umbra-opacity)); color=
: var(--jp-ui-font-color1); background-color: var(--jp-layout-color3); }

.jupyter-widget-colortag { color: var(--jp-inverse-ui-font-color1); }

.jupyter-widget-colortag.mod-active { color: var(--jp-inverse-ui-font-color=
0); }

.jupyter-widget-taginput { color: var(--jp-ui-font-color0); background-colo=
r: var(--jp-layout-color0); cursor: text; text-align: left; }

.jupyter-widget-taginput:focus { outline: none; }

.jupyter-widget-tag-close { margin-left: var(--jp-widgets-inline-margin); p=
adding: 2px 0px 2px 2px; }

.jupyter-widget-tag-close:hover { cursor: pointer; }

.jupyter-widget-tag.mod-primary { color: var(--jp-inverse-ui-font-color1); =
background-color: var(--jp-brand-color1); }

.jupyter-widget-tag.mod-primary.mod-active { color: var(--jp-inverse-ui-fon=
t-color0); background-color: var(--jp-brand-color0); }

.jupyter-widget-tag.mod-success { color: var(--jp-inverse-ui-font-color1); =
background-color: var(--jp-success-color1); }

.jupyter-widget-tag.mod-success.mod-active { color: var(--jp-inverse-ui-fon=
t-color0); background-color: var(--jp-success-color0); }

.jupyter-widget-tag.mod-info { color: var(--jp-inverse-ui-font-color1); bac=
kground-color: var(--jp-info-color1); }

.jupyter-widget-tag.mod-info.mod-active { color: var(--jp-inverse-ui-font-c=
olor0); background-color: var(--jp-info-color0); }

.jupyter-widget-tag.mod-warning { color: var(--jp-inverse-ui-font-color1); =
background-color: var(--jp-warn-color1); }

.jupyter-widget-tag.mod-warning.mod-active { color: var(--jp-inverse-ui-fon=
t-color0); background-color: var(--jp-warn-color0); }

.jupyter-widget-tag.mod-danger { color: var(--jp-inverse-ui-font-color1); b=
ackground-color: var(--jp-error-color1); }

.jupyter-widget-tag.mod-danger.mod-active { color: var(--jp-inverse-ui-font=
-color0); background-color: var(--jp-error-color0); }

.jupyter-button { padding: 0px 10px; display: inline-block; white-space: no=
wrap; overflow: hidden; text-overflow: ellipsis; text-align: center; font-s=
ize: var(--jp-widgets-font-size); cursor: pointer; height: var(--jp-widgets=
-inline-height); line-height: var(--jp-widgets-inline-height); box-shadow: =
none; color: var(--jp-ui-font-color1); background-color: var(--jp-layout-co=
lor2); border: none; user-select: none; }

.jupyter-button i.fa { margin-right: var(--jp-widgets-inline-margin); point=
er-events: none; }

.jupyter-button:empty::before { content: "=E2=80=8B"; }

.jupyter-widgets.jupyter-button:disabled { opacity: var(--jp-widgets-disabl=
ed-opacity); }

.jupyter-button i.fa.center { margin-right: 0px; }

.jupyter-button:hover:enabled, .jupyter-button:focus:enabled { box-shadow: =
0 2px 2px 0 rgba(0, 0, 0, var(--md-shadow-key-penumbra-opacity)),
    0 3px 1px -2px rgba(0, 0, 0, var(--md-shadow-key-umbra-opacity)),
    0 1px 5px 0 rgba(0, 0, 0, var(--md-shadow-ambient-shadow-opacity)); }

.jupyter-button:active, .jupyter-button.mod-active { box-shadow: 0 4px 5px =
0 rgba(0, 0, 0, var(--md-shadow-key-penumbra-opacity)),
    0 1px 10px 0 rgba(0, 0, 0, var(--md-shadow-ambient-shadow-opacity)),
    0 2px 4px -1px rgba(0, 0, 0, var(--md-shadow-key-umbra-opacity)); color=
: var(--jp-ui-font-color1); background-color: var(--jp-layout-color3); }

.jupyter-button:focus:enabled { outline: 1px solid var(--jp-widgets-input-f=
ocus-border-color); }

.jupyter-button.mod-primary { color: var(--jp-ui-inverse-font-color1); back=
ground-color: var(--jp-brand-color1); }

.jupyter-button.mod-primary.mod-active { color: var(--jp-ui-inverse-font-co=
lor0); background-color: var(--jp-brand-color0); }

.jupyter-button.mod-primary:active { color: var(--jp-ui-inverse-font-color0=
); background-color: var(--jp-brand-color0); }

.jupyter-button.mod-success { color: var(--jp-ui-inverse-font-color1); back=
ground-color: var(--jp-success-color1); }

.jupyter-button.mod-success.mod-active { color: var(--jp-ui-inverse-font-co=
lor0); background-color: var(--jp-success-color0); }

.jupyter-button.mod-success:active { color: var(--jp-ui-inverse-font-color0=
); background-color: var(--jp-success-color0); }

.jupyter-button.mod-info { color: var(--jp-ui-inverse-font-color1); backgro=
und-color: var(--jp-info-color1); }

.jupyter-button.mod-info.mod-active { color: var(--jp-ui-inverse-font-color=
0); background-color: var(--jp-info-color0); }

.jupyter-button.mod-info:active { color: var(--jp-ui-inverse-font-color0); =
background-color: var(--jp-info-color0); }

.jupyter-button.mod-warning { color: var(--jp-ui-inverse-font-color1); back=
ground-color: var(--jp-warn-color1); }

.jupyter-button.mod-warning.mod-active { color: var(--jp-ui-inverse-font-co=
lor0); background-color: var(--jp-warn-color0); }

.jupyter-button.mod-warning:active { color: var(--jp-ui-inverse-font-color0=
); background-color: var(--jp-warn-color0); }

.jupyter-button.mod-danger { color: var(--jp-ui-inverse-font-color1); backg=
round-color: var(--jp-error-color1); }

.jupyter-button.mod-danger.mod-active { color: var(--jp-ui-inverse-font-col=
or0); background-color: var(--jp-error-color0); }

.jupyter-button.mod-danger:active { color: var(--jp-ui-inverse-font-color0)=
; background-color: var(--jp-error-color0); }

.widget-button, .widget-toggle-button, .widget-upload, .jupyter-widget-butt=
on, .jupyter-widget-toggle-button, .jupyter-widget-upload { width: var(--jp=
-widgets-inline-width-short); }

.jupyter-widgets label { margin-bottom: initial; }

.widget-label-basic, .jupyter-widget-label-basic { color: var(--jp-widgets-=
label-color); font-size: var(--jp-widgets-font-size); overflow: hidden; tex=
t-overflow: ellipsis; white-space: nowrap; line-height: var(--jp-widgets-in=
line-height); }

.widget-label, .jupyter-widget-label { color: var(--jp-widgets-label-color)=
; font-size: var(--jp-widgets-font-size); overflow: hidden; text-overflow: =
ellipsis; white-space: nowrap; line-height: var(--jp-widgets-inline-height)=
; }

.widget-inline-hbox .widget-label, .jupyter-widget-inline-hbox .jupyter-wid=
get-label { color: var(--jp-widgets-label-color); text-align: right; margin=
-right: calc(var(--jp-widgets-inline-margin) * 2); width: var(--jp-widgets-=
inline-label-width); flex-shrink: 0; }

.widget-inline-vbox .widget-label, .jupyter-widget-inline-vbox .jupyter-wid=
get-label { color: var(--jp-widgets-label-color); text-align: center; line-=
height: var(--jp-widgets-inline-height); }

.widget-readout, .jupyter-widget-readout { color: var(--jp-widgets-readout-=
color); font-size: var(--jp-widgets-font-size); height: var(--jp-widgets-in=
line-height); line-height: var(--jp-widgets-inline-height); overflow: hidde=
n; white-space: nowrap; text-align: center; }

.widget-readout.overflow, .jupyter-widget-readout.overflow { box-shadow: rg=
ba(0, 0, 0, 0.2) 0px 2px 2px 0px, rgba(0, 0, 0, 0.14) 0px 3px 1px -2px, rgb=
a(0, 0, 0, 0.12) 0px 1px 5px 0px; }

.widget-inline-hbox .widget-readout, .jupyter-widget-inline-hbox .jupyter-w=
idget-readout { text-align: center; max-width: var(--jp-widgets-inline-widt=
h-short); min-width: var(--jp-widgets-inline-width-tiny); margin-left: var(=
--jp-widgets-inline-margin); }

.widget-inline-vbox .widget-readout, .jupyter-widget-inline-vbox .jupyter-w=
idget-readout { margin-top: var(--jp-widgets-inline-margin); width: inherit=
; }

.widget-checkbox, .jupyter-widget-checkbox { width: var(--jp-widgets-inline=
-width); height: var(--jp-widgets-inline-height); line-height: var(--jp-wid=
gets-inline-height); }

.widget-checkbox input[type=3D"checkbox"], .jupyter-widget-checkbox input[t=
ype=3D"checkbox"] { margin: 0px calc(var(--jp-widgets-inline-margin) * 2) 0=
px 0px; line-height: var(--jp-widgets-inline-height); font-size: large; fle=
x-grow: 1; flex-shrink: 0; align-self: center; }

.widget-valid, .jupyter-widget-valid { height: var(--jp-widgets-inline-heig=
ht); line-height: var(--jp-widgets-inline-height); width: var(--jp-widgets-=
inline-width-short); font-size: var(--jp-widgets-font-size); }

.widget-valid i, .jupyter-widget-valid i { line-height: var(--jp-widgets-in=
line-height); margin-right: var(--jp-widgets-inline-margin); margin-left: v=
ar(--jp-widgets-inline-margin); }

.widget-valid.mod-valid i, .jupyter-widget-valid.mod-valid i { color: green=
; }

.widget-valid.mod-invalid i, .jupyter-widget-valid.mod-invalid i { color: r=
ed; }

.widget-valid.mod-valid .widget-valid-readout, .jupyter-widget-valid.mod-va=
lid .jupyter-widget-valid-readout { display: none; }

.widget-textarea, .widget-text, .jupyter-widget-textarea, .jupyter-widget-t=
ext { width: var(--jp-widgets-inline-width); }

.widget-text input[type=3D"text"], .widget-text input[type=3D"number"], .wi=
dget-text input[type=3D"password"], .jupyter-widget-text input[type=3D"text=
"], .jupyter-widget-text input[type=3D"number"], .jupyter-widget-text input=
[type=3D"password"] { height: var(--jp-widgets-inline-height); }

.widget-text input[type=3D"text"]:disabled, .widget-text input[type=3D"numb=
er"]:disabled, .widget-text input[type=3D"password"]:disabled, .widget-text=
area textarea:disabled, .jupyter-widget-text input[type=3D"text"]:disabled,=
 .jupyter-widget-text input[type=3D"number"]:disabled, .jupyter-widget-text=
 input[type=3D"password"]:disabled, .jupyter-widget-textarea textarea:disab=
led { opacity: var(--jp-widgets-disabled-opacity); }

.widget-text input[type=3D"text"], .widget-text input[type=3D"number"], .wi=
dget-text input[type=3D"password"], .widget-textarea textarea, .jupyter-wid=
get-text input[type=3D"text"], .jupyter-widget-text input[type=3D"number"],=
 .jupyter-widget-text input[type=3D"password"], .jupyter-widget-textarea te=
xtarea { box-sizing: border-box; border: var(--jp-widgets-input-border-widt=
h) solid
    var(--jp-widgets-input-border-color); background-color: var(--jp-widget=
s-input-background-color); color: var(--jp-widgets-input-color); font-size:=
 var(--jp-widgets-font-size); flex-grow: 1; min-width: 0px; flex-shrink: 1;=
 outline: none !important; }

.widget-text input[type=3D"text"], .widget-text input[type=3D"password"], .=
widget-textarea textarea, .jupyter-widget-text input[type=3D"text"], .jupyt=
er-widget-text input[type=3D"password"], .jupyter-widget-textarea textarea =
{ padding: var(--jp-widgets-input-padding)
    calc(var(--jp-widgets-input-padding) * 2); }

.widget-text input[type=3D"number"], .jupyter-widget-text input[type=3D"num=
ber"] { padding: var(--jp-widgets-input-padding) 0 var(--jp-widgets-input-p=
adding)
    calc(var(--jp-widgets-input-padding) * 2); }

.widget-textarea textarea, .jupyter-widget-textarea textarea { height: inhe=
rit; width: inherit; }

.widget-text input:focus, .widget-textarea textarea:focus, .jupyter-widget-=
text input:focus, .jupyter-widget-textarea textarea:focus { border-color: v=
ar(--jp-widgets-input-focus-border-color); }

.widget-hslider, .jupyter-widget-hslider { width: var(--jp-widgets-inline-w=
idth); height: var(--jp-widgets-inline-height); line-height: var(--jp-widge=
ts-inline-height); align-items: center; }

.widgets-slider .slider-container, .jupyter-widgets-slider .slider-containe=
r { overflow: visible; }

.widget-hslider .slider-container, .jupyter-widget-hslider .slider-containe=
r { margin-left: calc(
    var(--jp-widgets-slider-handle-size) / 2 - 2 *
      var(--jp-widgets-slider-border-width)
  ); margin-right: calc(
    var(--jp-widgets-slider-handle-size) / 2 - 2 *
      var(--jp-widgets-slider-border-width)
  ); flex: 1 1 var(--jp-widgets-inline-width-short); }

.widget-vbox .widget-label, .jupyter-widget-vbox .jupyter-widget-label { he=
ight: var(--jp-widgets-inline-height); line-height: var(--jp-widgets-inline=
-height); }

.widget-vslider, .jupyter-widget-vslider { height: var(--jp-widgets-vertica=
l-height); width: var(--jp-widgets-inline-width-tiny); }

.widget-vslider .slider-container, .jupyter-widget-vslider .slider-containe=
r { flex: 1 1 var(--jp-widgets-inline-width-short); margin-left: auto; marg=
in-right: auto; margin-bottom: calc(
    var(--jp-widgets-slider-handle-size) / 2 - 2 *
      var(--jp-widgets-slider-border-width)
  ); margin-top: calc(
    var(--jp-widgets-slider-handle-size) / 2 - 2 *
      var(--jp-widgets-slider-border-width)
  ); display: flex; flex-direction: column; }

.progress-bar { transition: none 0s ease 0s; }

.progress-bar { height: var(--jp-widgets-inline-height); }

.progress-bar { background-color: var(--jp-brand-color1); }

.progress-bar-success { background-color: var(--jp-success-color1); }

.progress-bar-info { background-color: var(--jp-info-color1); }

.progress-bar-warning { background-color: var(--jp-warn-color1); }

.progress-bar-danger { background-color: var(--jp-error-color1); }

.progress { background-color: var(--jp-layout-color2); border: none; box-sh=
adow: none; }

.widget-hprogress, .jupyter-widget-hprogress { height: var(--jp-widgets-inl=
ine-height); line-height: var(--jp-widgets-inline-height); width: var(--jp-=
widgets-inline-width); align-items: center; }

.widget-hprogress .progress, .jupyter-widget-hprogress .progress { flex-gro=
w: 1; margin-top: var(--jp-widgets-input-padding); margin-bottom: var(--jp-=
widgets-input-padding); align-self: stretch; height: initial; }

.widget-vprogress, .jupyter-widget-vprogress { height: var(--jp-widgets-ver=
tical-height); width: var(--jp-widgets-inline-width-tiny); }

.widget-vprogress .progress, .jupyter-widget-vprogress .progress { flex-gro=
w: 1; width: var(--jp-widgets-progress-thickness); margin-left: auto; margi=
n-right: auto; margin-bottom: 0px; }

.widget-dropdown, .jupyter-widget-dropdown { height: var(--jp-widgets-inlin=
e-height); width: var(--jp-widgets-inline-width); line-height: var(--jp-wid=
gets-inline-height); }

.widget-dropdown > select, .jupyter-widget-dropdown > select { padding-righ=
t: 20px; border: var(--jp-widgets-input-border-width) solid
    var(--jp-widgets-input-border-color); border-radius: 0px; height: inher=
it; flex: 1 1 var(--jp-widgets-inline-width-short); min-width: 0px; box-siz=
ing: border-box; box-shadow: none; background-color: var(--jp-widgets-input=
-background-color); color: var(--jp-widgets-input-color); font-size: var(--=
jp-widgets-font-size); vertical-align: top; padding-left: calc(var(--jp-wid=
gets-input-padding) * 2); appearance: none; background-repeat: no-repeat; b=
ackground-size: 20px; background-position: right center; background-image: =
var(--jp-widgets-dropdown-arrow); outline: none !important; }

.widget-dropdown > select:focus, .jupyter-widget-dropdown > select:focus { =
border-color: var(--jp-widgets-input-focus-border-color); }

.widget-dropdown > select:disabled, .jupyter-widget-dropdown > select:disab=
led { opacity: var(--jp-widgets-disabled-opacity); }

.widget-select, .jupyter-widget-select { width: var(--jp-widgets-inline-wid=
th); line-height: var(--jp-widgets-inline-height); align-items: flex-start;=
 }

.widget-select > select, .jupyter-widget-select > select { border: var(--jp=
-widgets-input-border-width) solid
    var(--jp-widgets-input-border-color); background-color: var(--jp-widget=
s-input-background-color); color: var(--jp-widgets-input-color); font-size:=
 var(--jp-widgets-font-size); flex: 1 1 var(--jp-widgets-inline-width-short=
); overflow: auto; height: inherit; padding-top: 5px; outline: none !import=
ant; }

.widget-select > select:focus, .jupyter-widget-select > select:focus { bord=
er-color: var(--jp-widgets-input-focus-border-color); }

.wiget-select > select > option, .jupyter-wiget-select > select > option { =
padding-left: var(--jp-widgets-input-padding); line-height: var(--jp-widget=
s-inline-height); padding-top: calc(
    var(--jp-widgets-inline-height) - var(--jp-widgets-font-size) / 2
  ); padding-bottom: calc(
    var(--jp-widgets-inline-height) - var(--jp-widgets-font-size) / 2
  ); }

.widget-toggle-buttons, .jupyter-widget-toggle-buttons { line-height: var(-=
-jp-widgets-inline-height); }

.widget-toggle-buttons .widget-toggle-button, .jupyter-widget-toggle-button=
s .jupyter-widget-toggle-button { margin-left: var(--jp-widgets-margin); ma=
rgin-right: var(--jp-widgets-margin); }

.widget-toggle-buttons .jupyter-button:disabled, .jupyter-widget-toggle-but=
tons .jupyter-button:disabled { opacity: var(--jp-widgets-disabled-opacity)=
; }

.widget-radio, .jupyter-widget-radio { width: var(--jp-widgets-inline-width=
); line-height: var(--jp-widgets-inline-height); }

.widget-radio-box, .jupyter-widget-radio-box { display: flex; flex-directio=
n: column; align-items: stretch; box-sizing: border-box; flex-grow: 1; marg=
in-bottom: var(--jp-widgets-radio-item-height-adjustment); }

.widget-radio-box label, .jupyter-widget-radio-box label { height: var(--jp=
-widgets-radio-item-height); line-height: var(--jp-widgets-radio-item-heigh=
t); font-size: var(--jp-widgets-font-size); }

.widget-radio-box input, .jupyter-widget-radio-box input { height: var(--jp=
-widgets-radio-item-height); line-height: var(--jp-widgets-radio-item-heigh=
t); margin: 0 calc(var(--jp-widgets-input-padding) * 2) 0 1px; float: left;=
 }

.widget-colorpicker, .jupyter-widget-colorpicker { width: var(--jp-widgets-=
inline-width); height: var(--jp-widgets-inline-height); line-height: var(--=
jp-widgets-inline-height); }

.widget-colorpicker > .widget-colorpicker-input, .jupyter-widget-colorpicke=
r > .jupyter-widget-colorpicker-input { flex-grow: 1; flex-shrink: 1; min-w=
idth: var(--jp-widgets-inline-width-tiny); }

.widget-colorpicker input[type=3D"color"], .jupyter-widget-colorpicker inpu=
t[type=3D"color"] { width: var(--jp-widgets-inline-height); height: var(--j=
p-widgets-inline-height); padding: 0px 2px; background: var(--jp-widgets-in=
put-background-color); color: var(--jp-widgets-input-color); border-top-col=
or: ; border-top-style: ; border-top-width: ; border-right-color: ; border-=
right-style: ; border-right-width: ; border-bottom-color: ; border-bottom-s=
tyle: ; border-bottom-width: ; border-image-source: ; border-image-slice: ;=
 border-image-width: ; border-image-outset: ; border-image-repeat: ; border=
-left: none; flex-grow: 0; flex-shrink: 0; box-sizing: border-box; align-se=
lf: stretch; outline: none !important; }

.widget-colorpicker.concise input[type=3D"color"], .jupyter-widget-colorpic=
ker.concise input[type=3D"color"] { border-left: var(--jp-widgets-input-bor=
der-width) solid
    var(--jp-widgets-input-border-color); }

.widget-colorpicker input[type=3D"color"]:focus, .widget-colorpicker input[=
type=3D"text"]:focus, .jupyter-widget-colorpicker input[type=3D"color"]:foc=
us, .jupyter-widget-colorpicker input[type=3D"text"]:focus { border-color: =
var(--jp-widgets-input-focus-border-color); }

.widget-colorpicker input[type=3D"text"], .jupyter-widget-colorpicker input=
[type=3D"text"] { flex-grow: 1; height: var(--jp-widgets-inline-height); li=
ne-height: var(--jp-widgets-inline-height); background: var(--jp-widgets-in=
put-background-color); color: var(--jp-widgets-input-color); border: var(--=
jp-widgets-input-border-width) solid
    var(--jp-widgets-input-border-color); font-size: var(--jp-widgets-font-=
size); padding: var(--jp-widgets-input-padding)
    calc(var(--jp-widgets-input-padding) * 2); min-width: 0px; flex-shrink:=
 1; box-sizing: border-box; outline: none !important; }

.widget-colorpicker input[type=3D"text"]:disabled, .jupyter-widget-colorpic=
ker input[type=3D"text"]:disabled { opacity: var(--jp-widgets-disabled-opac=
ity); }

.widget-datepicker, .jupyter-widget-datepicker { width: var(--jp-widgets-in=
line-width); height: var(--jp-widgets-inline-height); line-height: var(--jp=
-widgets-inline-height); }

.widget-datepicker input[type=3D"date"], .jupyter-widget-datepicker input[t=
ype=3D"date"] { flex-grow: 1; flex-shrink: 1; min-width: 0px; height: var(-=
-jp-widgets-inline-height); border: var(--jp-widgets-input-border-width) so=
lid
    var(--jp-widgets-input-border-color); background-color: var(--jp-widget=
s-input-background-color); color: var(--jp-widgets-input-color); font-size:=
 var(--jp-widgets-font-size); padding: var(--jp-widgets-input-padding)
    calc(var(--jp-widgets-input-padding) * 2); box-sizing: border-box; outl=
ine: none !important; }

.widget-datepicker input[type=3D"date"]:focus, .jupyter-widget-datepicker i=
nput[type=3D"date"]:focus { border-color: var(--jp-widgets-input-focus-bord=
er-color); }

.widget-datepicker input[type=3D"date"]:invalid, .jupyter-widget-datepicker=
 input[type=3D"date"]:invalid { border-color: var(--jp-warn-color1); }

.widget-datepicker input[type=3D"date"]:disabled, .jupyter-widget-datepicke=
r input[type=3D"date"]:disabled { opacity: var(--jp-widgets-disabled-opacit=
y); }

.widget-play, .jupyter-widget-play { width: var(--jp-widgets-inline-width-s=
hort); display: flex; align-items: stretch; }

.widget-play .jupyter-button, .jupyter-widget-play .jupyter-button { flex-g=
row: 1; height: auto; }

.widget-play .jupyter-button:disabled, .jupyter-widget-play .jupyter-button=
:disabled { opacity: var(--jp-widgets-disabled-opacity); }

.jupyter-widgets.widget-tab, .jupyter-widgets.jupyter-widget-tab { display:=
 flex; flex-direction: column; }

.jupyter-widgets.widget-tab > .p-TabBar, .jupyter-widgets.jupyter-widget-ta=
b > .p-TabBar, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar { overflow:=
 visible; }

.jupyter-widgets.widget-tab > .p-TabBar > .p-TabBar-content, .jupyter-widge=
ts.jupyter-widget-tab > .p-TabBar > .p-TabBar-content, .jupyter-widgets.jup=
yter-widget-tab > .lm-TabBar > .lm-TabBar-content { align-items: flex-end; =
min-width: 0px; min-height: 0px; }

.jupyter-widgets.widget-tab > .widget-tab-contents, .jupyter-widgets.jupyte=
r-widget-tab > .widget-tab-contents { width: 100%; box-sizing: border-box; =
margin: 0px; background: var(--jp-layout-color1); color: var(--jp-ui-font-c=
olor1); border: var(--jp-border-width) solid var(--jp-border-color1); paddi=
ng: var(--jp-widgets-container-padding); flex-grow: 1; overflow: auto; }

.jupyter-widgets.widget-tab > .p-TabBar, .jupyter-widgets.jupyter-widget-ta=
b > .p-TabBar, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar { font: var=
(--jp-widgets-font-size) Helvetica, Arial, sans-serif; min-height: calc(
    var(--jp-widgets-horizontal-tab-height) + var(--jp-border-width)
  ); }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab, .jupyter-widgets.jup=
yter-widget-tab > .p-TabBar .p-TabBar-tab, .jupyter-widgets.jupyter-widget-=
tab > .lm-TabBar .lm-TabBar-tab { flex: 0 1 var(--jp-widgets-horizontal-tab=
-width); min-width: 35px; min-height: calc(
    var(--jp-widgets-horizontal-tab-height) + var(--jp-border-width)
  ); line-height: var(--jp-widgets-horizontal-tab-height); margin-left: cal=
c(-1 * var(--jp-border-width)); padding: 0px 10px; background: var(--jp-lay=
out-color2); color: var(--jp-ui-font-color2); border-top-color: ; border-to=
p-style: ; border-top-width: ; border-right-color: ; border-right-style: ; =
border-right-width: ; border-left-color: ; border-left-style: ; border-left=
-width: ; border-image-source: ; border-image-slice: ; border-image-width: =
; border-image-outset: ; border-image-repeat: ; border-bottom: none; positi=
on: relative; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab.p-mod-current, .jupyt=
er-widgets.jupyter-widget-tab > .p-TabBar .p-TabBar-tab.p-mod-current, .jup=
yter-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-tab.lm-mod-current =
{ color: var(--jp-ui-font-color0); background: var(--jp-layout-color1); min=
-height: calc(
    var(--jp-widgets-horizontal-tab-height) + 2 * var(--jp-border-width)
  ); transform: translateY(var(--jp-border-width)); overflow: visible; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab.p-mod-current::before=
, .jupyter-widgets.jupyter-widget-tab > .p-TabBar .p-TabBar-tab.p-mod-curre=
nt::before, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-tab=
.lm-mod-current::before { position: absolute; top: calc(-1 * var(--jp-borde=
r-width)); left: calc(-1 * var(--jp-border-width)); content: ""; height: va=
r(--jp-widgets-horizontal-tab-top-border); width: calc(100% + 2 * var(--jp-=
border-width)); background: var(--jp-brand-color1); }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab:first-child, .jupyter=
-widgets.jupyter-widget-tab > .p-TabBar .p-TabBar-tab:first-child, .jupyter=
-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-tab:first-child { margi=
n-left: 0px; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tab:hover:not(.p-mod-curr=
ent), .jupyter-widgets.jupyter-widget-tab > .p-TabBar .p-TabBar-tab:hover:n=
ot(.p-mod-current), .jupyter-widgets.jupyter-widget-tab > .lm-TabBar .lm-Ta=
bBar-tab:hover:not(.lm-mod-current) { background: var(--jp-layout-color1); =
color: var(--jp-ui-font-color1); }

.jupyter-widgets.widget-tab > .p-TabBar .p-mod-closable > .p-TabBar-tabClos=
eIcon, .jupyter-widgets.jupyter-widget-tab > .p-TabBar .p-mod-closable > .p=
-TabBar-tabCloseIcon, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar .lm-=
mod-closable > .lm-TabBar-tabCloseIcon { margin-left: 4px; }

.jupyter-widgets.widget-tab > .p-TabBar .p-mod-closable > .p-TabBar-tabClos=
eIcon::before, .jupyter-widgets.jupyter-widget-widget-tab > .p-TabBar .p-mo=
d-closable > .p-TabBar-tabCloseIcon::before, .jupyter-widgets.jupyter-widge=
t-tab > .lm-TabBar .lm-mod-closable > .lm-TabBar-tabCloseIcon::before { fon=
t-family: FontAwesome; content: "=EF=80=8D"; }

.jupyter-widgets.widget-tab > .p-TabBar .p-TabBar-tabIcon, .jupyter-widgets=
.widget-tab > .p-TabBar .p-TabBar-tabLabel, .jupyter-widgets.widget-tab > .=
p-TabBar .p-TabBar-tabCloseIcon, .jupyter-widgets.jupyter-widget-tab > .p-T=
abBar .p-TabBar-tabIcon, .jupyter-widgets.jupyter-widget-tab > .p-TabBar .p=
-TabBar-tabLabel, .jupyter-widgets.jupyter-widget-tab > .p-TabBar .p-TabBar=
-tabCloseIcon, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-=
tabIcon, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-tabLab=
el, .jupyter-widgets.jupyter-widget-tab > .lm-TabBar .lm-TabBar-tabCloseIco=
n { line-height: var(--jp-widgets-horizontal-tab-height); }

.jupyter-widget-Collapse { display: flex; flex-direction: column; align-ite=
ms: stretch; }

.jupyter-widget-Collapse-header { cursor: pointer; color: var(--jp-ui-font-=
color2); background-color: var(--jp-layout-color2); border: var(--jp-widget=
s-border-width) solid var(--jp-border-color1); padding: calc(var(--jp-widge=
ts-container-padding) * 2 / 3)
    var(--jp-widgets-container-padding); font-weight: bold; }

.jupyter-widget-Collapse-header:hover { background-color: var(--jp-layout-c=
olor1); color: var(--jp-ui-font-color1); }

.jupyter-widget-Collapse-open > .jupyter-widget-Collapse-header { backgroun=
d-color: var(--jp-layout-color1); color: var(--jp-ui-font-color0); cursor: =
default; border-bottom: none; }

.jupyter-widget-Collapse-contents { padding: var(--jp-widgets-container-pad=
ding); background-color: var(--jp-layout-color1); color: var(--jp-ui-font-c=
olor1); border-left: var(--jp-widgets-border-width) solid var(--jp-border-c=
olor1); border-right: var(--jp-widgets-border-width) solid var(--jp-border-=
color1); border-bottom: var(--jp-widgets-border-width) solid var(--jp-borde=
r-color1); overflow: auto; }

.jupyter-widget-Accordion { display: flex; flex-direction: column; align-it=
ems: stretch; }

.jupyter-widget-Accordion .jupyter-widget-Collapse { margin-bottom: 0px; }

.jupyter-widget-Accordion .jupyter-widget-Collapse + .jupyter-widget-Collap=
se { margin-top: 4px; }

.widget-html, .widget-htmlmath, .jupyter-widget-html, .jupyter-widget-htmlm=
ath { font-size: var(--jp-widgets-font-size); }

.widget-html > .widget-html-content, .widget-htmlmath > .widget-html-conten=
t, .jupyter-widget-html > .jupyter-widget-html-content, .jupyter-widget-htm=
lmath > .jupyter-widget-html-content { align-self: stretch; flex-grow: 1; f=
lex-shrink: 1; line-height: var(--jp-widgets-inline-height); position: rela=
tive; }

.widget-image, .jupyter-widget-image { max-width: 100%; height: auto; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: cid:css-89c58381-a5d3-49a2-96b6-758f3f064c43@mhtml.blink

@charset "utf-8";
=0A
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/static/components/jquery-ui/dist/themes/smoothness/jquery-ui.min.css?v=32f9dcde0cd9843f2b66d34c1c9928b59a5d7ef007ba7a6a6a790b3e78f7857a698444d7a716dfaf8fa834c3b3175efd258bbc07cfc4aabb86769b07e5f358c3

@charset "utf-8";

.ui-helper-hidden { display: none; }

.ui-helper-hidden-accessible { border: 0px; clip: rect(0px, 0px, 0px, 0px);=
 height: 1px; margin: -1px; overflow: hidden; padding: 0px; position: absol=
ute; width: 1px; }

.ui-helper-reset { margin: 0px; padding: 0px; border: 0px; outline: 0px; li=
ne-height: 1.3; text-decoration: none; font-size: 100%; list-style: none; }

.ui-helper-clearfix::before, .ui-helper-clearfix::after { content: ""; disp=
lay: table; border-collapse: collapse; }

.ui-helper-clearfix::after { clear: both; }

.ui-helper-zfix { width: 100%; height: 100%; top: 0px; left: 0px; position:=
 absolute; opacity: 0; }

.ui-front { z-index: 100; }

.ui-state-disabled { pointer-events: none; cursor: default !important; }

.ui-icon { display: inline-block; vertical-align: middle; margin-top: -0.25=
em; position: relative; text-indent: -99999px; overflow: hidden; background=
-repeat: no-repeat; }

.ui-widget-icon-block { left: 50%; margin-left: -8px; display: block; }

.ui-widget-overlay { position: fixed; top: 0px; left: 0px; width: 100%; hei=
ght: 100%; }

.ui-accordion .ui-accordion-header { display: block; cursor: pointer; posit=
ion: relative; margin: 2px 0px 0px; padding: 0.5em 0.5em 0.5em 0.7em; font-=
size: 100%; }

.ui-accordion .ui-accordion-content { padding: 1em 2.2em; border-top: 0px; =
overflow: auto; }

.ui-autocomplete { position: absolute; top: 0px; left: 0px; cursor: default=
; }

.ui-menu { list-style: none; padding: 0px; margin: 0px; display: block; out=
line: 0px; }

.ui-menu .ui-menu { position: absolute; }

.ui-menu .ui-menu-item { margin: 0px; cursor: pointer; list-style-image: ur=
l("data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAA=
IBRAA7"); }

.ui-menu .ui-menu-item-wrapper { position: relative; padding: 3px 1em 3px 0=
.4em; }

.ui-menu .ui-menu-divider { margin: 5px 0px; height: 0px; font-size: 0px; l=
ine-height: 0; border-width: 1px 0px 0px; }

.ui-menu .ui-state-focus, .ui-menu .ui-state-active { margin: -1px; }

.ui-menu-icons { position: relative; }

.ui-menu-icons .ui-menu-item-wrapper { padding-left: 2em; }

.ui-menu .ui-icon { position: absolute; top: 0px; bottom: 0px; left: 0.2em;=
 margin: auto 0px; }

.ui-menu .ui-menu-icon { left: auto; right: 0px; }

.ui-button { padding: 0.4em 1em; display: inline-block; position: relative;=
 line-height: normal; margin-right: 0.1em; cursor: pointer; vertical-align:=
 middle; text-align: center; user-select: none; overflow: visible; }

.ui-button, .ui-button:link, .ui-button:visited, .ui-button:hover, .ui-butt=
on:active { text-decoration: none; }

.ui-button-icon-only { width: 2em; box-sizing: border-box; text-indent: -99=
99px; white-space: nowrap; }

input.ui-button.ui-button-icon-only { text-indent: 0px; }

.ui-button-icon-only .ui-icon { position: absolute; top: 50%; left: 50%; ma=
rgin-top: -8px; margin-left: -8px; }

.ui-button.ui-icon-notext .ui-icon { padding: 0px; width: 2.1em; height: 2.=
1em; text-indent: -9999px; white-space: nowrap; }

input.ui-button.ui-icon-notext .ui-icon { width: auto; height: auto; text-i=
ndent: 0px; white-space: normal; padding: 0.4em 1em; }

.ui-controlgroup { vertical-align: middle; display: inline-block; }

.ui-controlgroup > .ui-controlgroup-item { float: left; margin-left: 0px; m=
argin-right: 0px; }

.ui-controlgroup > .ui-controlgroup-item:focus, .ui-controlgroup > .ui-cont=
rolgroup-item.ui-visual-focus { z-index: 9999; }

.ui-controlgroup-vertical > .ui-controlgroup-item { display: block; float: =
none; width: 100%; margin-top: 0px; margin-bottom: 0px; text-align: left; }

.ui-controlgroup-vertical .ui-controlgroup-item { box-sizing: border-box; }

.ui-controlgroup .ui-controlgroup-label { padding: 0.4em 1em; }

.ui-controlgroup .ui-controlgroup-label span { font-size: 80%; }

.ui-controlgroup-horizontal .ui-controlgroup-label + .ui-controlgroup-item =
{ border-left: none; }

.ui-controlgroup-vertical .ui-controlgroup-label + .ui-controlgroup-item { =
border-top: none; }

.ui-controlgroup-horizontal .ui-controlgroup-label.ui-widget-content { bord=
er-right: none; }

.ui-controlgroup-vertical .ui-controlgroup-label.ui-widget-content { border=
-bottom: none; }

.ui-controlgroup-vertical .ui-spinner-input { width: calc(100% - 2.4em); }

.ui-controlgroup-vertical .ui-spinner .ui-spinner-up { border-top-style: so=
lid; }

.ui-checkboxradio-label .ui-icon-background { box-shadow: rgb(204, 204, 204=
) 1px 1px 1px inset; border-radius: 0.12em; border: none; }

.ui-checkboxradio-radio-label .ui-icon-background { width: 16px; height: 16=
px; border-radius: 1em; overflow: visible; border: none; }

.ui-checkboxradio-radio-label.ui-checkboxradio-checked .ui-icon, .ui-checkb=
oxradio-radio-label.ui-checkboxradio-checked:hover .ui-icon { background-im=
age: none; width: 8px; height: 8px; border-width: 4px; border-style: solid;=
 }

.ui-checkboxradio-disabled { pointer-events: none; }

.ui-datepicker { width: 17em; padding: 0.2em 0.2em 0px; display: none; }

.ui-datepicker .ui-datepicker-header { position: relative; padding: 0.2em 0=
px; }

.ui-datepicker .ui-datepicker-prev, .ui-datepicker .ui-datepicker-next { po=
sition: absolute; top: 2px; width: 1.8em; height: 1.8em; }

.ui-datepicker .ui-datepicker-prev-hover, .ui-datepicker .ui-datepicker-nex=
t-hover { top: 1px; }

.ui-datepicker .ui-datepicker-prev { left: 2px; }

.ui-datepicker .ui-datepicker-next { right: 2px; }

.ui-datepicker .ui-datepicker-prev-hover { left: 1px; }

.ui-datepicker .ui-datepicker-next-hover { right: 1px; }

.ui-datepicker .ui-datepicker-prev span, .ui-datepicker .ui-datepicker-next=
 span { display: block; position: absolute; left: 50%; margin-left: -8px; t=
op: 50%; margin-top: -8px; }

.ui-datepicker .ui-datepicker-title { margin: 0px 2.3em; line-height: 1.8em=
; text-align: center; }

.ui-datepicker .ui-datepicker-title select { font-size: 1em; margin: 1px 0p=
x; }

.ui-datepicker select.ui-datepicker-month, .ui-datepicker select.ui-datepic=
ker-year { width: 45%; }

.ui-datepicker table { width: 100%; font-size: 0.9em; border-collapse: coll=
apse; margin: 0px 0px 0.4em; }

.ui-datepicker th { padding: 0.7em 0.3em; text-align: center; font-weight: =
bold; border: 0px; }

.ui-datepicker td { border: 0px; padding: 1px; }

.ui-datepicker td span, .ui-datepicker td a { display: block; padding: 0.2e=
m; text-align: right; text-decoration: none; }

.ui-datepicker .ui-datepicker-buttonpane { background-image: none; margin: =
0.7em 0px 0px; padding: 0px 0.2em; border-left: 0px; border-right: 0px; bor=
der-bottom: 0px; }

.ui-datepicker .ui-datepicker-buttonpane button { float: right; margin: 0.5=
em 0.2em 0.4em; cursor: pointer; padding: 0.2em 0.6em 0.3em; width: auto; o=
verflow: visible; }

.ui-datepicker .ui-datepicker-buttonpane button.ui-datepicker-current { flo=
at: left; }

.ui-datepicker.ui-datepicker-multi { width: auto; }

.ui-datepicker-multi .ui-datepicker-group { float: left; }

.ui-datepicker-multi .ui-datepicker-group table { width: 95%; margin: 0px a=
uto 0.4em; }

.ui-datepicker-multi-2 .ui-datepicker-group { width: 50%; }

.ui-datepicker-multi-3 .ui-datepicker-group { width: 33.3%; }

.ui-datepicker-multi-4 .ui-datepicker-group { width: 25%; }

.ui-datepicker-multi .ui-datepicker-group-last .ui-datepicker-header, .ui-d=
atepicker-multi .ui-datepicker-group-middle .ui-datepicker-header { border-=
left-width: 0px; }

.ui-datepicker-multi .ui-datepicker-buttonpane { clear: left; }

.ui-datepicker-row-break { clear: both; width: 100%; font-size: 0px; }

.ui-datepicker-rtl { direction: rtl; }

.ui-datepicker-rtl .ui-datepicker-prev { right: 2px; left: auto; }

.ui-datepicker-rtl .ui-datepicker-next { left: 2px; right: auto; }

.ui-datepicker-rtl .ui-datepicker-prev:hover { right: 1px; left: auto; }

.ui-datepicker-rtl .ui-datepicker-next:hover { left: 1px; right: auto; }

.ui-datepicker-rtl .ui-datepicker-buttonpane { clear: right; }

.ui-datepicker-rtl .ui-datepicker-buttonpane button { float: left; }

.ui-datepicker-rtl .ui-datepicker-buttonpane button.ui-datepicker-current, =
.ui-datepicker-rtl .ui-datepicker-group { float: right; }

.ui-datepicker-rtl .ui-datepicker-group-last .ui-datepicker-header, .ui-dat=
epicker-rtl .ui-datepicker-group-middle .ui-datepicker-header { border-righ=
t-width: 0px; border-left-width: 1px; }

.ui-datepicker .ui-icon { display: block; text-indent: -99999px; overflow: =
hidden; background-repeat: no-repeat; left: 0.5em; top: 0.3em; }

.ui-dialog { position: absolute; top: 0px; left: 0px; padding: 0.2em; outli=
ne: 0px; }

.ui-dialog .ui-dialog-titlebar { padding: 0.4em 1em; position: relative; }

.ui-dialog .ui-dialog-title { float: left; margin: 0.1em 0px; white-space: =
nowrap; width: 90%; overflow: hidden; text-overflow: ellipsis; }

.ui-dialog .ui-dialog-titlebar-close { position: absolute; right: 0.3em; to=
p: 50%; width: 20px; margin: -10px 0px 0px; padding: 1px; height: 20px; }

.ui-dialog .ui-dialog-content { position: relative; border: 0px; padding: 0=
.5em 1em; background: none; overflow: auto; }

.ui-dialog .ui-dialog-buttonpane { text-align: left; border-width: 1px 0px =
0px; background-image: none; margin-top: 0.5em; padding: 0.3em 1em 0.5em 0.=
4em; }

.ui-dialog .ui-dialog-buttonpane .ui-dialog-buttonset { float: right; }

.ui-dialog .ui-dialog-buttonpane button { margin: 0.5em 0.4em 0.5em 0px; cu=
rsor: pointer; }

.ui-dialog .ui-resizable-n { height: 2px; top: 0px; }

.ui-dialog .ui-resizable-e { width: 2px; right: 0px; }

.ui-dialog .ui-resizable-s { height: 2px; bottom: 0px; }

.ui-dialog .ui-resizable-w { width: 2px; left: 0px; }

.ui-dialog .ui-resizable-se, .ui-dialog .ui-resizable-sw, .ui-dialog .ui-re=
sizable-ne, .ui-dialog .ui-resizable-nw { width: 7px; height: 7px; }

.ui-dialog .ui-resizable-se { right: 0px; bottom: 0px; }

.ui-dialog .ui-resizable-sw { left: 0px; bottom: 0px; }

.ui-dialog .ui-resizable-ne { right: 0px; top: 0px; }

.ui-dialog .ui-resizable-nw { left: 0px; top: 0px; }

.ui-draggable .ui-dialog-titlebar { cursor: move; }

.ui-draggable-handle { touch-action: none; }

.ui-resizable { position: relative; }

.ui-resizable-handle { position: absolute; font-size: 0.1px; display: block=
; touch-action: none; }

.ui-resizable-disabled .ui-resizable-handle, .ui-resizable-autohide .ui-res=
izable-handle { display: none; }

.ui-resizable-n { cursor: n-resize; height: 7px; width: 100%; top: -5px; le=
ft: 0px; }

.ui-resizable-s { cursor: s-resize; height: 7px; width: 100%; bottom: -5px;=
 left: 0px; }

.ui-resizable-e { cursor: e-resize; width: 7px; right: -5px; top: 0px; heig=
ht: 100%; }

.ui-resizable-w { cursor: w-resize; width: 7px; left: -5px; top: 0px; heigh=
t: 100%; }

.ui-resizable-se { cursor: se-resize; width: 12px; height: 12px; right: 1px=
; bottom: 1px; }

.ui-resizable-sw { cursor: sw-resize; width: 9px; height: 9px; left: -5px; =
bottom: -5px; }

.ui-resizable-nw { cursor: nw-resize; width: 9px; height: 9px; left: -5px; =
top: -5px; }

.ui-resizable-ne { cursor: ne-resize; width: 9px; height: 9px; right: -5px;=
 top: -5px; }

.ui-progressbar { height: 2em; text-align: left; overflow: hidden; }

.ui-progressbar .ui-progressbar-value { margin: -1px; height: 100%; }

.ui-progressbar .ui-progressbar-overlay { background: url("data:image/gif;b=
ase64,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
=3D=3D"); height: 100%; opacity: 0.25; }

.ui-progressbar-indeterminate .ui-progressbar-value { background-image: non=
e; }

.ui-selectable { touch-action: none; }

.ui-selectable-helper { position: absolute; z-index: 100; border: 1px dotte=
d black; }

.ui-selectmenu-menu { padding: 0px; margin: 0px; position: absolute; top: 0=
px; left: 0px; display: none; }

.ui-selectmenu-menu .ui-menu { overflow: hidden auto; padding-bottom: 1px; =
}

.ui-selectmenu-menu .ui-menu .ui-selectmenu-optgroup { font-size: 1em; font=
-weight: bold; line-height: 1.5; padding: 2px 0.4em; margin: 0.5em 0px 0px;=
 height: auto; border: 0px; }

.ui-selectmenu-open { display: block; }

.ui-selectmenu-text { display: block; margin-right: 20px; overflow: hidden;=
 text-overflow: ellipsis; }

.ui-selectmenu-button.ui-button { text-align: left; white-space: nowrap; wi=
dth: 14em; }

.ui-selectmenu-icon.ui-icon { float: right; margin-top: 0px; }

.ui-slider { position: relative; text-align: left; }

.ui-slider .ui-slider-handle { position: absolute; z-index: 2; width: 1.2em=
; height: 1.2em; cursor: pointer; touch-action: none; }

.ui-slider .ui-slider-range { position: absolute; z-index: 1; font-size: 0.=
7em; display: block; border: 0px; background-position: 0px 0px; }

.ui-slider.ui-state-disabled .ui-slider-handle, .ui-slider.ui-state-disable=
d .ui-slider-range { filter: inherit; }

.ui-slider-horizontal { height: 0.8em; }

.ui-slider-horizontal .ui-slider-handle { top: -0.3em; margin-left: -0.6em;=
 }

.ui-slider-horizontal .ui-slider-range { top: 0px; height: 100%; }

.ui-slider-horizontal .ui-slider-range-min { left: 0px; }

.ui-slider-horizontal .ui-slider-range-max { right: 0px; }

.ui-slider-vertical { width: 0.8em; height: 100px; }

.ui-slider-vertical .ui-slider-handle { left: -0.3em; margin-left: 0px; mar=
gin-bottom: -0.6em; }

.ui-slider-vertical .ui-slider-range { left: 0px; width: 100%; }

.ui-slider-vertical .ui-slider-range-min { bottom: 0px; }

.ui-slider-vertical .ui-slider-range-max { top: 0px; }

.ui-sortable-handle { touch-action: none; }

.ui-spinner { position: relative; display: inline-block; overflow: hidden; =
padding: 0px; vertical-align: middle; }

.ui-spinner-input { border: none; background: none; color: inherit; padding=
: 0.222em 0px; margin: 0.2em 2em 0.2em 0.4em; vertical-align: middle; }

.ui-spinner-button { width: 1.6em; height: 50%; font-size: 0.5em; padding: =
0px; margin: 0px; text-align: center; position: absolute; cursor: default; =
display: block; overflow: hidden; right: 0px; }

.ui-spinner a.ui-spinner-button { border-top-style: none; border-bottom-sty=
le: none; border-right-style: none; }

.ui-spinner-up { top: 0px; }

.ui-spinner-down { bottom: 0px; }

.ui-tabs { position: relative; padding: 0.2em; }

.ui-tabs .ui-tabs-nav { margin: 0px; padding: 0.2em 0.2em 0px; }

.ui-tabs .ui-tabs-nav li { list-style: none; float: left; position: relativ=
e; top: 0px; margin: 1px 0.2em 0px 0px; border-bottom-width: 0px; padding: =
0px; white-space: nowrap; }

.ui-tabs .ui-tabs-nav .ui-tabs-anchor { float: left; padding: 0.5em 1em; te=
xt-decoration: none; }

.ui-tabs .ui-tabs-nav li.ui-tabs-active { margin-bottom: -1px; padding-bott=
om: 1px; }

.ui-tabs .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor, .ui-tabs .ui-tabs-=
nav li.ui-state-disabled .ui-tabs-anchor, .ui-tabs .ui-tabs-nav li.ui-tabs-=
loading .ui-tabs-anchor { cursor: text; }

.ui-tabs-collapsible .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor { curso=
r: pointer; }

.ui-tabs .ui-tabs-panel { display: block; border-width: 0px; padding: 1em 1=
.4em; background: none; }

.ui-tooltip { padding: 8px; position: absolute; z-index: 9999; max-width: 3=
00px; }

body .ui-tooltip { border-width: 2px; }

.ui-widget { font-family: Verdana, Arial, sans-serif; font-size: 1.1em; }

.ui-widget .ui-widget { font-size: 1em; }

.ui-widget input, .ui-widget select, .ui-widget textarea, .ui-widget button=
 { font-family: Verdana, Arial, sans-serif; font-size: 1em; }

.ui-widget.ui-widget-content { border: 1px solid rgb(211, 211, 211); }

.ui-widget-content { border: 1px solid rgb(170, 170, 170); background: rgb(=
255, 255, 255); color: rgb(34, 34, 34); }

.ui-widget-content a { color: rgb(34, 34, 34); }

.ui-widget-header { border: 1px solid rgb(170, 170, 170); background: url("=
images/ui-bg_highlight-soft_75_cccccc_1x100.png") 50% 50% repeat-x rgb(204,=
 204, 204); color: rgb(34, 34, 34); font-weight: bold; }

.ui-widget-header a { color: rgb(34, 34, 34); }

.ui-state-default, .ui-widget-content .ui-state-default, .ui-widget-header =
.ui-state-default, .ui-button, html .ui-button.ui-state-disabled:hover, htm=
l .ui-button.ui-state-disabled:active { border: 1px solid rgb(211, 211, 211=
); background: url("images/ui-bg_glass_75_e6e6e6_1x400.png") 50% 50% repeat=
-x rgb(230, 230, 230); font-weight: normal; color: rgb(85, 85, 85); }

.ui-state-default a, .ui-state-default a:link, .ui-state-default a:visited,=
 a.ui-button, a:link.ui-button, a:visited.ui-button, .ui-button { color: rg=
b(85, 85, 85); text-decoration: none; }

.ui-state-hover, .ui-widget-content .ui-state-hover, .ui-widget-header .ui-=
state-hover, .ui-state-focus, .ui-widget-content .ui-state-focus, .ui-widge=
t-header .ui-state-focus, .ui-button:hover, .ui-button:focus { border: 1px =
solid rgb(153, 153, 153); background: url("images/ui-bg_glass_75_dadada_1x4=
00.png") 50% 50% repeat-x rgb(218, 218, 218); font-weight: normal; color: r=
gb(33, 33, 33); }

.ui-state-hover a, .ui-state-hover a:hover, .ui-state-hover a:link, .ui-sta=
te-hover a:visited, .ui-state-focus a, .ui-state-focus a:hover, .ui-state-f=
ocus a:link, .ui-state-focus a:visited, a.ui-button:hover, a.ui-button:focu=
s { color: rgb(33, 33, 33); text-decoration: none; }

.ui-visual-focus { box-shadow: rgb(94, 158, 214) 0px 0px 3px 1px; }

.ui-state-active, .ui-widget-content .ui-state-active, .ui-widget-header .u=
i-state-active, a.ui-button:active, .ui-button:active, .ui-button.ui-state-=
active:hover { border: 1px solid rgb(170, 170, 170); background: url("image=
s/ui-bg_glass_65_ffffff_1x400.png") 50% 50% repeat-x rgb(255, 255, 255); fo=
nt-weight: normal; color: rgb(33, 33, 33); }

.ui-icon-background, .ui-state-active .ui-icon-background { border: rgb(170=
, 170, 170); background-color: rgb(33, 33, 33); }

.ui-state-active a, .ui-state-active a:link, .ui-state-active a:visited { c=
olor: rgb(33, 33, 33); text-decoration: none; }

.ui-state-highlight, .ui-widget-content .ui-state-highlight, .ui-widget-hea=
der .ui-state-highlight { border: 1px solid rgb(252, 239, 161); background:=
 url("images/ui-bg_glass_55_fbf9ee_1x400.png") 50% 50% repeat-x rgb(251, 24=
9, 238); color: rgb(54, 54, 54); }

.ui-state-checked { border: 1px solid rgb(252, 239, 161); background: rgb(2=
51, 249, 238); }

.ui-state-highlight a, .ui-widget-content .ui-state-highlight a, .ui-widget=
-header .ui-state-highlight a { color: rgb(54, 54, 54); }

.ui-state-error, .ui-widget-content .ui-state-error, .ui-widget-header .ui-=
state-error { border: 1px solid rgb(205, 10, 10); background: url("images/u=
i-bg_glass_95_fef1ec_1x400.png") 50% 50% repeat-x rgb(254, 241, 236); color=
: rgb(205, 10, 10); }

.ui-state-error a, .ui-widget-content .ui-state-error a, .ui-widget-header =
.ui-state-error a { color: rgb(205, 10, 10); }

.ui-state-error-text, .ui-widget-content .ui-state-error-text, .ui-widget-h=
eader .ui-state-error-text { color: rgb(205, 10, 10); }

.ui-priority-primary, .ui-widget-content .ui-priority-primary, .ui-widget-h=
eader .ui-priority-primary { font-weight: bold; }

.ui-priority-secondary, .ui-widget-content .ui-priority-secondary, .ui-widg=
et-header .ui-priority-secondary { opacity: 0.7; font-weight: normal; }

.ui-state-disabled, .ui-widget-content .ui-state-disabled, .ui-widget-heade=
r .ui-state-disabled { opacity: 0.35; background-image: none; }

.ui-state-disabled .ui-icon { }

.ui-icon { width: 16px; height: 16px; }

.ui-icon, .ui-widget-content .ui-icon { background-image: url("images/ui-ic=
ons_222222_256x240.png"); }

.ui-widget-header .ui-icon { background-image: url("images/ui-icons_222222_=
256x240.png"); }

.ui-state-hover .ui-icon, .ui-state-focus .ui-icon, .ui-button:hover .ui-ic=
on, .ui-button:focus .ui-icon { background-image: url("images/ui-icons_4545=
45_256x240.png"); }

.ui-state-active .ui-icon, .ui-button:active .ui-icon { background-image: u=
rl("images/ui-icons_454545_256x240.png"); }

.ui-state-highlight .ui-icon, .ui-button .ui-state-highlight.ui-icon { back=
ground-image: url("images/ui-icons_2e83ff_256x240.png"); }

.ui-state-error .ui-icon, .ui-state-error-text .ui-icon { background-image:=
 url("images/ui-icons_cd0a0a_256x240.png"); }

.ui-button .ui-icon { background-image: url("images/ui-icons_888888_256x240=
.png"); }

.ui-icon-blank.ui-icon-blank.ui-icon-blank { background-image: none; }

.ui-icon-caret-1-n { background-position: 0px 0px; }

.ui-icon-caret-1-ne { background-position: -16px 0px; }

.ui-icon-caret-1-e { background-position: -32px 0px; }

.ui-icon-caret-1-se { background-position: -48px 0px; }

.ui-icon-caret-1-s { background-position: -65px 0px; }

.ui-icon-caret-1-sw { background-position: -80px 0px; }

.ui-icon-caret-1-w { background-position: -96px 0px; }

.ui-icon-caret-1-nw { background-position: -112px 0px; }

.ui-icon-caret-2-n-s { background-position: -128px 0px; }

.ui-icon-caret-2-e-w { background-position: -144px 0px; }

.ui-icon-triangle-1-n { background-position: 0px -16px; }

.ui-icon-triangle-1-ne { background-position: -16px -16px; }

.ui-icon-triangle-1-e { background-position: -32px -16px; }

.ui-icon-triangle-1-se { background-position: -48px -16px; }

.ui-icon-triangle-1-s { background-position: -65px -16px; }

.ui-icon-triangle-1-sw { background-position: -80px -16px; }

.ui-icon-triangle-1-w { background-position: -96px -16px; }

.ui-icon-triangle-1-nw { background-position: -112px -16px; }

.ui-icon-triangle-2-n-s { background-position: -128px -16px; }

.ui-icon-triangle-2-e-w { background-position: -144px -16px; }

.ui-icon-arrow-1-n { background-position: 0px -32px; }

.ui-icon-arrow-1-ne { background-position: -16px -32px; }

.ui-icon-arrow-1-e { background-position: -32px -32px; }

.ui-icon-arrow-1-se { background-position: -48px -32px; }

.ui-icon-arrow-1-s { background-position: -65px -32px; }

.ui-icon-arrow-1-sw { background-position: -80px -32px; }

.ui-icon-arrow-1-w { background-position: -96px -32px; }

.ui-icon-arrow-1-nw { background-position: -112px -32px; }

.ui-icon-arrow-2-n-s { background-position: -128px -32px; }

.ui-icon-arrow-2-ne-sw { background-position: -144px -32px; }

.ui-icon-arrow-2-e-w { background-position: -160px -32px; }

.ui-icon-arrow-2-se-nw { background-position: -176px -32px; }

.ui-icon-arrowstop-1-n { background-position: -192px -32px; }

.ui-icon-arrowstop-1-e { background-position: -208px -32px; }

.ui-icon-arrowstop-1-s { background-position: -224px -32px; }

.ui-icon-arrowstop-1-w { background-position: -240px -32px; }

.ui-icon-arrowthick-1-n { background-position: 1px -48px; }

.ui-icon-arrowthick-1-ne { background-position: -16px -48px; }

.ui-icon-arrowthick-1-e { background-position: -32px -48px; }

.ui-icon-arrowthick-1-se { background-position: -48px -48px; }

.ui-icon-arrowthick-1-s { background-position: -64px -48px; }

.ui-icon-arrowthick-1-sw { background-position: -80px -48px; }

.ui-icon-arrowthick-1-w { background-position: -96px -48px; }

.ui-icon-arrowthick-1-nw { background-position: -112px -48px; }

.ui-icon-arrowthick-2-n-s { background-position: -128px -48px; }

.ui-icon-arrowthick-2-ne-sw { background-position: -144px -48px; }

.ui-icon-arrowthick-2-e-w { background-position: -160px -48px; }

.ui-icon-arrowthick-2-se-nw { background-position: -176px -48px; }

.ui-icon-arrowthickstop-1-n { background-position: -192px -48px; }

.ui-icon-arrowthickstop-1-e { background-position: -208px -48px; }

.ui-icon-arrowthickstop-1-s { background-position: -224px -48px; }

.ui-icon-arrowthickstop-1-w { background-position: -240px -48px; }

.ui-icon-arrowreturnthick-1-w { background-position: 0px -64px; }

.ui-icon-arrowreturnthick-1-n { background-position: -16px -64px; }

.ui-icon-arrowreturnthick-1-e { background-position: -32px -64px; }

.ui-icon-arrowreturnthick-1-s { background-position: -48px -64px; }

.ui-icon-arrowreturn-1-w { background-position: -64px -64px; }

.ui-icon-arrowreturn-1-n { background-position: -80px -64px; }

.ui-icon-arrowreturn-1-e { background-position: -96px -64px; }

.ui-icon-arrowreturn-1-s { background-position: -112px -64px; }

.ui-icon-arrowrefresh-1-w { background-position: -128px -64px; }

.ui-icon-arrowrefresh-1-n { background-position: -144px -64px; }

.ui-icon-arrowrefresh-1-e { background-position: -160px -64px; }

.ui-icon-arrowrefresh-1-s { background-position: -176px -64px; }

.ui-icon-arrow-4 { background-position: 0px -80px; }

.ui-icon-arrow-4-diag { background-position: -16px -80px; }

.ui-icon-extlink { background-position: -32px -80px; }

.ui-icon-newwin { background-position: -48px -80px; }

.ui-icon-refresh { background-position: -64px -80px; }

.ui-icon-shuffle { background-position: -80px -80px; }

.ui-icon-transfer-e-w { background-position: -96px -80px; }

.ui-icon-transferthick-e-w { background-position: -112px -80px; }

.ui-icon-folder-collapsed { background-position: 0px -96px; }

.ui-icon-folder-open { background-position: -16px -96px; }

.ui-icon-document { background-position: -32px -96px; }

.ui-icon-document-b { background-position: -48px -96px; }

.ui-icon-note { background-position: -64px -96px; }

.ui-icon-mail-closed { background-position: -80px -96px; }

.ui-icon-mail-open { background-position: -96px -96px; }

.ui-icon-suitcase { background-position: -112px -96px; }

.ui-icon-comment { background-position: -128px -96px; }

.ui-icon-person { background-position: -144px -96px; }

.ui-icon-print { background-position: -160px -96px; }

.ui-icon-trash { background-position: -176px -96px; }

.ui-icon-locked { background-position: -192px -96px; }

.ui-icon-unlocked { background-position: -208px -96px; }

.ui-icon-bookmark { background-position: -224px -96px; }

.ui-icon-tag { background-position: -240px -96px; }

.ui-icon-home { background-position: 0px -112px; }

.ui-icon-flag { background-position: -16px -112px; }

.ui-icon-calendar { background-position: -32px -112px; }

.ui-icon-cart { background-position: -48px -112px; }

.ui-icon-pencil { background-position: -64px -112px; }

.ui-icon-clock { background-position: -80px -112px; }

.ui-icon-disk { background-position: -96px -112px; }

.ui-icon-calculator { background-position: -112px -112px; }

.ui-icon-zoomin { background-position: -128px -112px; }

.ui-icon-zoomout { background-position: -144px -112px; }

.ui-icon-search { background-position: -160px -112px; }

.ui-icon-wrench { background-position: -176px -112px; }

.ui-icon-gear { background-position: -192px -112px; }

.ui-icon-heart { background-position: -208px -112px; }

.ui-icon-star { background-position: -224px -112px; }

.ui-icon-link { background-position: -240px -112px; }

.ui-icon-cancel { background-position: 0px -128px; }

.ui-icon-plus { background-position: -16px -128px; }

.ui-icon-plusthick { background-position: -32px -128px; }

.ui-icon-minus { background-position: -48px -128px; }

.ui-icon-minusthick { background-position: -64px -128px; }

.ui-icon-close { background-position: -80px -128px; }

.ui-icon-closethick { background-position: -96px -128px; }

.ui-icon-key { background-position: -112px -128px; }

.ui-icon-lightbulb { background-position: -128px -128px; }

.ui-icon-scissors { background-position: -144px -128px; }

.ui-icon-clipboard { background-position: -160px -128px; }

.ui-icon-copy { background-position: -176px -128px; }

.ui-icon-contact { background-position: -192px -128px; }

.ui-icon-image { background-position: -208px -128px; }

.ui-icon-video { background-position: -224px -128px; }

.ui-icon-script { background-position: -240px -128px; }

.ui-icon-alert { background-position: 0px -144px; }

.ui-icon-info { background-position: -16px -144px; }

.ui-icon-notice { background-position: -32px -144px; }

.ui-icon-help { background-position: -48px -144px; }

.ui-icon-check { background-position: -64px -144px; }

.ui-icon-bullet { background-position: -80px -144px; }

.ui-icon-radio-on { background-position: -96px -144px; }

.ui-icon-radio-off { background-position: -112px -144px; }

.ui-icon-pin-w { background-position: -128px -144px; }

.ui-icon-pin-s { background-position: -144px -144px; }

.ui-icon-play { background-position: 0px -160px; }

.ui-icon-pause { background-position: -16px -160px; }

.ui-icon-seek-next { background-position: -32px -160px; }

.ui-icon-seek-prev { background-position: -48px -160px; }

.ui-icon-seek-end { background-position: -64px -160px; }

.ui-icon-seek-start { background-position: -80px -160px; }

.ui-icon-seek-first { background-position: -80px -160px; }

.ui-icon-stop { background-position: -96px -160px; }

.ui-icon-eject { background-position: -112px -160px; }

.ui-icon-volume-off { background-position: -128px -160px; }

.ui-icon-volume-on { background-position: -144px -160px; }

.ui-icon-power { background-position: 0px -176px; }

.ui-icon-signal-diag { background-position: -16px -176px; }

.ui-icon-signal { background-position: -32px -176px; }

.ui-icon-battery-0 { background-position: -48px -176px; }

.ui-icon-battery-1 { background-position: -64px -176px; }

.ui-icon-battery-2 { background-position: -80px -176px; }

.ui-icon-battery-3 { background-position: -96px -176px; }

.ui-icon-circle-plus { background-position: 0px -192px; }

.ui-icon-circle-minus { background-position: -16px -192px; }

.ui-icon-circle-close { background-position: -32px -192px; }

.ui-icon-circle-triangle-e { background-position: -48px -192px; }

.ui-icon-circle-triangle-s { background-position: -64px -192px; }

.ui-icon-circle-triangle-w { background-position: -80px -192px; }

.ui-icon-circle-triangle-n { background-position: -96px -192px; }

.ui-icon-circle-arrow-e { background-position: -112px -192px; }

.ui-icon-circle-arrow-s { background-position: -128px -192px; }

.ui-icon-circle-arrow-w { background-position: -144px -192px; }

.ui-icon-circle-arrow-n { background-position: -160px -192px; }

.ui-icon-circle-zoomin { background-position: -176px -192px; }

.ui-icon-circle-zoomout { background-position: -192px -192px; }

.ui-icon-circle-check { background-position: -208px -192px; }

.ui-icon-circlesmall-plus { background-position: 0px -208px; }

.ui-icon-circlesmall-minus { background-position: -16px -208px; }

.ui-icon-circlesmall-close { background-position: -32px -208px; }

.ui-icon-squaresmall-plus { background-position: -48px -208px; }

.ui-icon-squaresmall-minus { background-position: -64px -208px; }

.ui-icon-squaresmall-close { background-position: -80px -208px; }

.ui-icon-grip-dotted-vertical { background-position: 0px -224px; }

.ui-icon-grip-dotted-horizontal { background-position: -16px -224px; }

.ui-icon-grip-solid-vertical { background-position: -32px -224px; }

.ui-icon-grip-solid-horizontal { background-position: -48px -224px; }

.ui-icon-gripsmall-diagonal-se { background-position: -64px -224px; }

.ui-icon-grip-diagonal-se { background-position: -80px -224px; }

.ui-corner-all, .ui-corner-top, .ui-corner-left, .ui-corner-tl { border-top=
-left-radius: 4px; }

.ui-corner-all, .ui-corner-top, .ui-corner-right, .ui-corner-tr { border-to=
p-right-radius: 4px; }

.ui-corner-all, .ui-corner-bottom, .ui-corner-left, .ui-corner-bl { border-=
bottom-left-radius: 4px; }

.ui-corner-all, .ui-corner-bottom, .ui-corner-right, .ui-corner-br { border=
-bottom-right-radius: 4px; }

.ui-widget-overlay { background: rgb(170, 170, 170); opacity: 0.3; }

.ui-widget-shadow { box-shadow: rgb(170, 170, 170) -8px -8px 8px; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/static/components/jquery-typeahead/dist/jquery.typeahead.min.css?v=5edf53bf6bb9c3b1ddafd8594825a7e2ed621f19423e569c985162742f63911c09eba2c529f8fb47aebf27fafdfe287d563347f58c1126b278189a18871b6a9a

@charset "utf-8";

.typeahead__container button, .typeahead__container input, .typeahead__cont=
ainer optgroup, .typeahead__container select, .typeahead__container textare=
a { font: inherit; margin: 0px; }

.typeahead__container optgroup { font-weight: 700; }

.typeahead__container button, .typeahead__container input { overflow: visib=
le; }

.typeahead__container button, .typeahead__container select { text-transform=
: none; }

.typeahead__container [type=3D"reset"], .typeahead__container [type=3D"subm=
it"], .typeahead__container button, .typeahead__container html [type=3D"but=
ton"] { appearance: button; }

.typeahead__container fieldset { border: 1px solid silver; margin: 0px 2px;=
 padding: 0.35em 0.625em 0.75em; }

.typeahead__container legend { box-sizing: border-box; color: inherit; disp=
lay: table; max-width: 100%; padding: 0px; white-space: normal; }

.typeahead__container textarea { overflow: auto; }

.typeahead__container [type=3D"checkbox"], .typeahead__container [type=3D"r=
adio"] { box-sizing: border-box; padding: 0px; }

.typeahead__container [type=3D"number"]::-webkit-inner-spin-button, .typeah=
ead__container [type=3D"number"]::-webkit-outer-spin-button { height: auto;=
 }

.typeahead__container ::-webkit-input-placeholder { color: inherit; opacity=
: 0.54; }

.typeahead__container ::-webkit-file-upload-button { appearance: button; fo=
nt: inherit; }

.typeahead__container { position: relative; font: 1rem Lato, "Helvetica Neu=
e", Arial, Helvetica, sans-serif; }

.typeahead__container * { box-sizing: border-box; outline: 0px; }

.typeahead__query { position: relative; z-index: 2; width: 100%; }

.typeahead__filter { position: relative; }

.typeahead__filter button { min-width: 100%; white-space: nowrap; }

.typeahead__filter button::after { display: inline-block; margin-left: 4px;=
 width: 0px; height: 0px; vertical-align: -2px; content: ""; border-width: =
4px; border-style: solid; border-top-color: initial; border-image: initial;=
 border-right-color: transparent; border-bottom-color: transparent; border-=
left-color: transparent; }

.typeahead__field { display: flex; position: relative; width: 100%; }

.typeahead__button button { border-top-right-radius: 2px; border-bottom-rig=
ht-radius: 2px; }

.typeahead__field { color: rgb(85, 85, 85); }

.typeahead__field .typeahead__hint, .typeahead__field [contenteditable], .t=
ypeahead__field input, .typeahead__field textarea { display: block; width: =
100%; line-height: 1.25; min-height: calc(2px + 2.25rem); padding: 0.5rem 0=
.75rem; background: rgb(255, 255, 255); border: 1px solid rgb(204, 204, 204=
); border-radius: 2px 0px 0px 2px; appearance: none; box-sizing: border-box=
; }

.typeahead__field .typeahead__hint:active, .typeahead__field .typeahead__hi=
nt:focus, .typeahead__field [contenteditable]:active, .typeahead__field [co=
ntenteditable]:focus, .typeahead__field input:active, .typeahead__field inp=
ut:focus, .typeahead__field textarea:active, .typeahead__field textarea:foc=
us { border-color: rgb(102, 175, 233); }

.typeahead__container.hint .typeahead__field [contenteditable], .typeahead_=
_container.hint .typeahead__field input, .typeahead__container.hint .typeah=
ead__field textarea { background: transparent; }

.typeahead__container.hint .typeahead__query > :last-child, .typeahead__hin=
t { background: rgb(255, 255, 255); }

.typeahead__container button { display: inline-block; margin-bottom: 0px; t=
ext-align: center; touch-action: manipulation; cursor: pointer; background-=
color: rgb(255, 255, 255); border: 1px solid rgb(204, 204, 204); line-heigh=
t: 1.25; padding: 0.5rem 0.75rem; user-select: none; color: rgb(85, 85, 85)=
; }

.typeahead__container button:focus, .typeahead__container button:hover { co=
lor: rgb(60, 60, 60); background-color: rgb(245, 245, 245); border-color: r=
gb(179, 179, 179); }

.typeahead__container button.active, .typeahead__container button:active { =
background-image: none; }

.typeahead__container button:active, .typeahead__container button:focus { b=
order-color: rgb(102, 175, 233); }

.typeahead__container button.disabled, .typeahead__container button[disable=
d], .typeahead__container input.disabled, .typeahead__container input[disab=
led] { cursor: not-allowed; pointer-events: none; opacity: 0.65; box-shadow=
: none; background-color: rgb(255, 255, 255); border-color: rgb(204, 204, 2=
04); }

.typeahead__container .typeahead__field .typeahead__hint, .typeahead__conta=
iner .typeahead__field .typeahead__label-container, .typeahead__container .=
typeahead__field [contenteditable], .typeahead__container .typeahead__field=
 input, .typeahead__container .typeahead__field textarea { padding-right: 3=
2px; }

.typeahead__button, .typeahead__filter { z-index: 1; }

.typeahead__button button, .typeahead__filter button { margin-left: -1px; b=
order-bottom-left-radius: 0px; border-top-left-radius: 0px; }

.typeahead__button:active, .typeahead__button:active button:active, .typeah=
ead__button:active button:focus, .typeahead__button:focus, .typeahead__butt=
on:focus button:active, .typeahead__button:focus button:focus, .typeahead__=
button:hover, .typeahead__button:hover button:active, .typeahead__button:ho=
ver button:focus, .typeahead__filter:active, .typeahead__filter:active butt=
on:active, .typeahead__filter:active button:focus, .typeahead__filter:focus=
, .typeahead__filter:focus button:active, .typeahead__filter:focus button:f=
ocus, .typeahead__filter:hover, .typeahead__filter:hover button:active, .ty=
peahead__filter:hover button:focus { z-index: 5; }

.typeahead__filter + .typeahead__button button { margin-left: -2px; }

.typeahead__container.filter .typeahead__filter { z-index: 5; }

.typeahead__dropdown, .typeahead__list { position: absolute; left: 0px; z-i=
ndex: 4; width: 100%; min-width: 160px; padding: 5px 0px; margin: 2px 0px 0=
px; list-style: none; text-align: left; background-color: rgb(255, 255, 255=
); border: 1px solid rgb(204, 204, 204); border-radius: 2px; background-cli=
p: padding-box; }

.typeahead__result.detached .typeahead__list { position: relative; z-index:=
 6; top: auto; left: auto; }

.typeahead__dropdown { right: 0px; left: auto; z-index: 5; }

.typeahead__list > li { position: relative; border-top: 1px solid rgb(204, =
204, 204); }

.typeahead__list > li:first-child { border-top: none; }

.typeahead__dropdown .typeahead__dropdown-item[disabled] > a, .typeahead__l=
ist .typeahead__item[disabled] > a { cursor: not-allowed; color: rgb(186, 1=
86, 186); background-color: rgb(250, 250, 250); }

.typeahead__dropdown .typeahead__dropdown-item > a, .typeahead__list .typea=
head__item > a { display: block; padding: 0.5rem 0.75rem; clear: both; colo=
r: rgb(51, 51, 51); text-decoration: none; }

.typeahead__dropdown .typeahead__dropdown-item:not([disabled]).active > a, =
.typeahead__dropdown .typeahead__dropdown-item:not([disabled]) > a:focus, .=
typeahead__dropdown .typeahead__dropdown-item:not([disabled]) > a:hover, .t=
ypeahead__list .typeahead__item:not([disabled]).active > a, .typeahead__lis=
t .typeahead__item:not([disabled]) > a:focus, .typeahead__list .typeahead__=
item:not([disabled]) > a:hover { background-color: rgb(245, 245, 245); colo=
r: rgb(60, 60, 60); }

.typeahead__list.empty > li { padding: 0.5rem 0.75rem; color: rgb(51, 51, 5=
1); }

.typeahead__list > .typeahead__group { border-color: rgb(191, 222, 246); fo=
nt-weight: 700; }

.typeahead__list > .typeahead__group:first-child { border-top: 1px solid rg=
b(191, 222, 246); }

.typeahead__list > .typeahead__group.active > a, .typeahead__list > .typeah=
ead__group > a, .typeahead__list > .typeahead__group > a:focus, .typeahead_=
_list > .typeahead__group > a:hover { cursor: default; color: rgb(23, 99, 1=
59); background: rgb(236, 245, 252); display: block; padding: 0.5rem 0.75re=
m; clear: both; text-decoration: none; }

.typeahead__list > li.typeahead__group + li.typeahead__item { border-color:=
 rgb(191, 222, 246); }

.typeahead__container.backdrop + .typeahead__backdrop, .typeahead__containe=
r.filter .typeahead__dropdown, .typeahead__container.hint .typeahead__hint,=
 .typeahead__container.result .typeahead__list { display: block !important;=
 }

.typeahead__container + .typeahead__backdrop, .typeahead__container .typeah=
ead__dropdown, .typeahead__container .typeahead__hint, .typeahead__containe=
r .typeahead__list { display: none !important; }

.typeahead__dropdown li:last-child { margin-top: 5px; padding-top: 5px; bor=
der-top: 1px solid rgb(204, 204, 204); }

.typeahead__cancel-button { user-select: none; position: absolute; right: 0=
px; cursor: pointer; line-height: 1.25; padding: 0.5rem 0.75rem; visibility=
: hidden; }

.typeahead__label .typeahead__cancel-button { visibility: visible; right: 4=
px; }

.typeahead__container.cancel:not(.loading) .typeahead__cancel-button, .type=
ahead__label .typeahead__cancel-button { visibility: visible; }

.typeahead__container.cancel:not(.loading) .typeahead__cancel-button:hover,=
 .typeahead__label .typeahead__cancel-button:hover { color: rgb(208, 2, 27)=
; }

.typeahead__search-icon { padding: 0px 1.25rem; width: 16px; height: 16px; =
background: url("data:image/svg+xml;charset=3Dutf8;base64,PD94bWwgdmVyc2lvb=
j0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pgo8IS0tIEdlbmVyYXRvcjogQWRvYmUgSWxs=
dXN0cmF0b3IgMTguMS4xLCBTVkcgRXhwb3J0IFBsdWctSW4gLiBTVkcgVmVyc2lvbjogNi4wMCB=
CdWlsZCAwKSAgLS0+CjxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bW=
xuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgdmVyc2lvbj0iMS4xIiBpZ=
D0iQ2FwYV8xIiB4PSIwcHgiIHk9IjBweCIgdmlld0JveD0iMCAwIDI1MC4zMTMgMjUwLjMxMyIg=
c3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgMjUwLjMxMyAyNTAuMzEzOyIgeG1sOnN=
wYWNlPSJwcmVzZXJ2ZSIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CjxnIGlkPSJTZWFyY2=
giPgoJPHBhdGggc3R5bGU9ImZpbGwtcnVsZTpldmVub2RkO2NsaXAtcnVsZTpldmVub2RkOyIgZ=
D0iTTI0NC4xODYsMjE0LjYwNGwtNTQuMzc5LTU0LjM3OGMtMC4yODktMC4yODktMC42MjgtMC40=
OTEtMC45My0wLjc2ICAgYzEwLjctMTYuMjMxLDE2Ljk0NS0zNS42NiwxNi45NDUtNTYuNTU0QzI=
wNS44MjIsNDYuMDc1LDE1OS43NDcsMCwxMDIuOTExLDBTMCw0Ni4wNzUsMCwxMDIuOTExICAgYz=
AsNTYuODM1LDQ2LjA3NCwxMDIuOTExLDEwMi45MSwxMDIuOTExYzIwLjg5NSwwLDQwLjMyMy02L=
jI0NSw1Ni41NTQtMTYuOTQ1YzAuMjY5LDAuMzAxLDAuNDcsMC42NCwwLjc1OSwwLjkyOWw1NC4z=
OCw1NC4zOCAgIGM4LjE2OSw4LjE2OCwyMS40MTMsOC4xNjgsMjkuNTgzLDBDMjUyLjM1NCwyMzY=
uMDE3LDI1Mi4zNTQsMjIyLjc3MywyNDQuMTg2LDIxNC42MDR6IE0xMDIuOTExLDE3MC4xNDYgIC=
BjLTM3LjEzNCwwLTY3LjIzNi0zMC4xMDItNjcuMjM2LTY3LjIzNWMwLTM3LjEzNCwzMC4xMDMtN=
jcuMjM2LDY3LjIzNi02Ny4yMzZjMzcuMTMyLDAsNjcuMjM1LDMwLjEwMyw2Ny4yMzUsNjcuMjM2=
ICAgQzE3MC4xNDYsMTQwLjA0NCwxNDAuMDQzLDE3MC4xNDYsMTAyLjkxMSwxNzAuMTQ2eiIgZml=
sbD0iIzU1NTU1NSIvPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+Cj=
xnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnP=
go8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+CjxnPgo8L2c+Cjwvc3ZnPgo=3D") 50%=
 center no-repeat scroll transparent; }

.typeahead__container.loading .typeahead__query::after, .typeahead__contain=
er.loading .typeahead__query::before { transition: all 0s linear 0s, opacit=
y 0.2s ease 0s; position: absolute; z-index: 3; content: ""; top: 50%; righ=
t: 0.55em; margin-top: -0.675rem; width: 1.35rem; height: 1.35rem; box-sizi=
ng: border-box; border-radius: 500rem; border-style: solid; border-width: 0=
.1em; }

.typeahead__container.loading .typeahead__query::before { border-color: rgb=
a(0, 0, 0, 0.35); }

.typeahead__container.loading .typeahead__query::after { animation: 0.6s li=
near 0s infinite normal none running a; border-color: rgb(255, 255, 255) tr=
ansparent transparent; box-shadow: transparent 0px 0px 0px 1px; }

@keyframes a {=20
  0% { transform: rotate(0deg); }
  100% { transform: rotate(1turn); }
}

.typeahead__label-container { list-style: none; position: absolute; padding=
-top: 0.375rem; padding-left: 6px; width: 100%; flex-wrap: wrap; display: f=
lex; }

.typeahead__label { display: flex; font-size: 0.875rem; position: relative;=
 background: rgb(236, 245, 252); border: 1px solid rgb(194, 224, 255); padd=
ing-left: 4px; border-radius: 2px; margin-right: 4px; margin-bottom: 0.375r=
em; }

.typeahead__label > * { align-self: center; }

.typeahead__label .typeahead__cancel-button { line-height: normal; height: =
auto; position: static; padding: calc(-1px + 0.25rem) 6px calc(1px + 0.25re=
m); margin-left: 4px; font-size: 0.875rem; border-left: 1px solid rgb(194, =
224, 255); }

.typeahead__label .typeahead__cancel-button:hover { background-color: rgb(2=
13, 233, 249); }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/static/components/bootstrap-tour/build/css/bootstrap-tour.min.css?v=95c93e52db61ab29625defe55361384ce6776a7d303b97da5a73fef5ddf8e391a6223599a0b58669476bd71645a4f0022df0517c88b0c05df80ba465e36f5417

@charset "utf-8";

.tour-backdrop { position: fixed; inset: 0px; z-index: 1100; background-col=
or: rgb(0, 0, 0); opacity: 0.8; }

.tour-step-backdrop { position: relative; z-index: 1101; background: inheri=
t; }

.tour-step-background { position: absolute; z-index: 1100; background: inhe=
rit; border-radius: 6px; }

.popover[class*=3D"tour-"] { z-index: 1100; }

.popover[class*=3D"tour-"] .popover-navigation { padding: 9px 14px; }

.popover[class*=3D"tour-"] .popover-navigation [data-role=3D"end"] { float:=
 right; }

.popover[class*=3D"tour-"] .popover-navigation [data-role=3D"prev"], .popov=
er[class*=3D"tour-"] .popover-navigation [data-role=3D"next"], .popover[cla=
ss*=3D"tour-"] .popover-navigation [data-role=3D"end"] { cursor: pointer; }

.popover[class*=3D"tour-"] .popover-navigation [data-role=3D"prev"].disable=
d, .popover[class*=3D"tour-"] .popover-navigation [data-role=3D"next"].disa=
bled, .popover[class*=3D"tour-"] .popover-navigation [data-role=3D"end"].di=
sabled { cursor: default; }

.popover[class*=3D"tour-"].orphan { position: fixed; margin-top: 0px; }

.popover[class*=3D"tour-"].orphan .arrow { display: none; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/static/components/codemirror/lib/codemirror.css?v=a545ad5e21a51420a7cb40234688eef087a5cf3798f64d7750291a8be0e9c760b8a1c9cbbbdcaa6470f2f385caa59e816f2640f609d29147f4762e27f69709e6

@charset "utf-8";

.CodeMirror { font-family: monospace; height: 300px; color: black; directio=
n: ltr; }

.CodeMirror-lines { padding: 4px 0px; }

.CodeMirror pre.CodeMirror-line, .CodeMirror pre.CodeMirror-line-like { pad=
ding: 0px 4px; }

.CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler { background-color:=
 white; }

.CodeMirror-gutters { border-right: 1px solid rgb(221, 221, 221); backgroun=
d-color: rgb(247, 247, 247); white-space: nowrap; }

.CodeMirror-linenumbers { }

.CodeMirror-linenumber { padding: 0px 3px 0px 5px; min-width: 20px; text-al=
ign: right; color: rgb(153, 153, 153); white-space: nowrap; }

.CodeMirror-guttermarker { color: black; }

.CodeMirror-guttermarker-subtle { color: rgb(153, 153, 153); }

.CodeMirror-cursor { border-left: 1px solid black; border-right: none; widt=
h: 0px; }

.CodeMirror div.CodeMirror-secondarycursor { border-left: 1px solid silver;=
 }

.cm-fat-cursor .CodeMirror-cursor { width: auto; background: rgb(119, 238, =
119); border: 0px !important; }

.cm-fat-cursor div.CodeMirror-cursors { z-index: 1; }

.cm-fat-cursor-mark { background-color: rgba(20, 255, 20, 0.5); animation: =
1.06s steps(1) 0s infinite normal none running blink; }

.cm-animate-fat-cursor { width: auto; border: 0px; animation: 1.06s steps(1=
) 0s infinite normal none running blink; background-color: rgb(119, 238, 11=
9); }

@-webkit-keyframes blink {=20
  0% { }
  50% { background-color: transparent; }
  100% { }
}

@keyframes blink {=20
  0% { }
  50% { background-color: transparent; }
  100% { }
}

.CodeMirror-overwrite .CodeMirror-cursor { }

.cm-tab { display: inline-block; text-decoration: inherit; }

.CodeMirror-rulers { position: absolute; inset: -50px 0px 0px; overflow: hi=
dden; }

.CodeMirror-ruler { border-left: 1px solid rgb(204, 204, 204); top: 0px; bo=
ttom: 0px; position: absolute; }

.cm-s-default .cm-header { color: blue; }

.cm-s-default .cm-quote { color: rgb(0, 153, 0); }

.cm-negative { color: rgb(221, 68, 68); }

.cm-positive { color: rgb(34, 153, 34); }

.cm-header, .cm-strong { font-weight: bold; }

.cm-em { font-style: italic; }

.cm-link { text-decoration: underline; }

.cm-strikethrough { text-decoration: line-through; }

.cm-s-default .cm-keyword { color: rgb(119, 0, 136); }

.cm-s-default .cm-atom { color: rgb(34, 17, 153); }

.cm-s-default .cm-number { color: rgb(17, 102, 68); }

.cm-s-default .cm-def { color: rgb(0, 0, 255); }

.cm-s-default .cm-variable, .cm-s-default .cm-punctuation, .cm-s-default .c=
m-property, .cm-s-default .cm-operator { }

.cm-s-default .cm-variable-2 { color: rgb(0, 85, 170); }

.cm-s-default .cm-variable-3, .cm-s-default .cm-type { color: rgb(0, 136, 8=
5); }

.cm-s-default .cm-comment { color: rgb(170, 85, 0); }

.cm-s-default .cm-string { color: rgb(170, 17, 17); }

.cm-s-default .cm-string-2 { color: rgb(255, 85, 0); }

.cm-s-default .cm-meta { color: rgb(85, 85, 85); }

.cm-s-default .cm-qualifier { color: rgb(85, 85, 85); }

.cm-s-default .cm-builtin { color: rgb(51, 0, 170); }

.cm-s-default .cm-bracket { color: rgb(153, 153, 119); }

.cm-s-default .cm-tag { color: rgb(17, 119, 0); }

.cm-s-default .cm-attribute { color: rgb(0, 0, 204); }

.cm-s-default .cm-hr { color: rgb(153, 153, 153); }

.cm-s-default .cm-link { color: rgb(0, 0, 204); }

.cm-s-default .cm-error { color: rgb(255, 0, 0); }

.cm-invalidchar { color: rgb(255, 0, 0); }

.CodeMirror-composing { border-bottom: 2px solid; }

div.CodeMirror span.CodeMirror-matchingbracket { color: rgb(0, 187, 0); }

div.CodeMirror span.CodeMirror-nonmatchingbracket { color: rgb(170, 34, 34)=
; }

.CodeMirror-matchingtag { background: rgba(255, 150, 0, 0.3); }

.CodeMirror-activeline-background { background: rgb(232, 242, 255); }

.CodeMirror { position: relative; overflow: hidden; background: white; }

.CodeMirror-scroll { margin-bottom: -50px; margin-right: -50px; padding-bot=
tom: 50px; height: 100%; outline: none; position: relative; overflow: scrol=
l !important; }

.CodeMirror-sizer { position: relative; border-right: 50px solid transparen=
t; }

.CodeMirror-vscrollbar, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-fille=
r, .CodeMirror-gutter-filler { position: absolute; z-index: 6; display: non=
e; outline: none; }

.CodeMirror-vscrollbar { right: 0px; top: 0px; overflow: hidden scroll; }

.CodeMirror-hscrollbar { bottom: 0px; left: 0px; overflow: scroll hidden; }

.CodeMirror-scrollbar-filler { right: 0px; bottom: 0px; }

.CodeMirror-gutter-filler { left: 0px; bottom: 0px; }

.CodeMirror-gutters { position: absolute; left: 0px; top: 0px; min-height: =
100%; z-index: 3; }

.CodeMirror-gutter { white-space: normal; height: 100%; display: inline-blo=
ck; vertical-align: top; margin-bottom: -50px; }

.CodeMirror-gutter-wrapper { position: absolute; z-index: 4; background: no=
ne !important; border: none !important; }

.CodeMirror-gutter-background { position: absolute; top: 0px; bottom: 0px; =
z-index: 4; }

.CodeMirror-gutter-elt { position: absolute; cursor: default; z-index: 4; }

.CodeMirror-gutter-wrapper ::selection { background-color: transparent; }

.CodeMirror-lines { cursor: text; min-height: 1px; }

.CodeMirror pre.CodeMirror-line, .CodeMirror pre.CodeMirror-line-like { bor=
der-radius: 0px; border-width: 0px; background: transparent; font-family: i=
nherit; font-size: inherit; margin: 0px; white-space: pre; overflow-wrap: n=
ormal; line-height: inherit; color: inherit; z-index: 2; position: relative=
; overflow: visible; -webkit-tap-highlight-color: transparent; font-variant=
-ligatures: contextual; }

.CodeMirror-wrap pre.CodeMirror-line, .CodeMirror-wrap pre.CodeMirror-line-=
like { overflow-wrap: break-word; white-space: pre-wrap; word-break: normal=
; }

.CodeMirror-linebackground { position: absolute; inset: 0px; z-index: 0; }

.CodeMirror-linewidget { position: relative; z-index: 2; padding: 0.1px; }

.CodeMirror-widget { }

.CodeMirror-rtl pre { direction: rtl; }

.CodeMirror-code { outline: none; }

.CodeMirror-scroll, .CodeMirror-sizer, .CodeMirror-gutter, .CodeMirror-gutt=
ers, .CodeMirror-linenumber { box-sizing: content-box; }

.CodeMirror-measure { position: absolute; width: 100%; height: 0px; overflo=
w: hidden; visibility: hidden; }

.CodeMirror-cursor { position: absolute; pointer-events: none; }

.CodeMirror-measure pre { position: static; }

div.CodeMirror-cursors { visibility: hidden; position: relative; z-index: 3=
; }

div.CodeMirror-dragcursors { visibility: visible; }

.CodeMirror-focused div.CodeMirror-cursors { visibility: visible; }

.CodeMirror-selected { background: rgb(217, 217, 217); }

.CodeMirror-focused .CodeMirror-selected { background: rgb(215, 212, 240); =
}

.CodeMirror-crosshair { cursor: crosshair; }

.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirro=
r-line > span > span::selection { background: rgb(215, 212, 240); }

.cm-searching { background-color: rgba(255, 255, 0, 0.4); }

.cm-force-border { padding-right: 0.1px; }

@media print {
  .CodeMirror div.CodeMirror-cursors { visibility: hidden; }
}

.cm-tab-wrap-hack::after { content: ""; }

span.CodeMirror-selectedtext { background: none; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/static/style/style.min.css?v=e1ab1c38b672063a6541baf468c83345cd0f509729783ec9b7ccb64073004f5f056110c82c28aefbf3dbf32e0e040f05b8f0420bc411b669ed3d4f07511812ca

@charset "utf-8";

html { font-family: sans-serif; text-size-adjust: 100%; }

body { margin: 0px; }

article, aside, details, figcaption, figure, footer, header, hgroup, main, =
menu, nav, section, summary { display: block; }

audio, canvas, progress, video { display: inline-block; vertical-align: bas=
eline; }

audio:not([controls]) { display: none; height: 0px; }

[hidden], template { display: none; }

a { background-color: transparent; }

a:active, a:hover { outline: 0px; }

abbr[title] { border-bottom: none; text-decoration: underline dotted; }

b, strong { font-weight: bold; }

dfn { font-style: italic; }

h1 { font-size: 2em; margin: 0.67em 0px; }

mark { background: rgb(255, 255, 0); color: rgb(0, 0, 0); }

small { font-size: 80%; }

sub, sup { font-size: 75%; line-height: 0; position: relative; vertical-ali=
gn: baseline; }

sup { top: -0.5em; }

sub { bottom: -0.25em; }

img { border: 0px; }

svg:not(:root) { overflow: hidden; }

figure { margin: 1em 40px; }

hr { box-sizing: content-box; height: 0px; }

pre { overflow: auto; }

code, kbd, pre, samp { font-family: monospace, monospace; font-size: 1em; }

button, input, optgroup, select, textarea { color: inherit; font: inherit; =
margin: 0px; }

button { overflow: visible; }

button, select { text-transform: none; }

button, html input[type=3D"button"], input[type=3D"reset"], input[type=3D"s=
ubmit"] { appearance: button; cursor: pointer; }

button[disabled], html input[disabled] { cursor: default; }

input { line-height: normal; }

input[type=3D"checkbox"], input[type=3D"radio"] { box-sizing: border-box; p=
adding: 0px; }

input[type=3D"number"]::-webkit-inner-spin-button, input[type=3D"number"]::=
-webkit-outer-spin-button { height: auto; }

input[type=3D"search"] { appearance: textfield; box-sizing: content-box; }

input[type=3D"search"]::-webkit-search-cancel-button, input[type=3D"search"=
]::-webkit-search-decoration { appearance: none; }

fieldset { border: 1px solid rgb(192, 192, 192); margin: 0px 2px; padding: =
0.35em 0.625em 0.75em; }

legend { border: 0px; padding: 0px; }

textarea { overflow: auto; }

optgroup { font-weight: bold; }

table { border-collapse: collapse; border-spacing: 0px; }

td, th { padding: 0px; }

@media print {
  *, ::before, ::after { text-shadow: none !important; background: transpar=
ent !important; box-shadow: none !important; }
  a, a:visited { text-decoration: underline; }
  a[href]::after { content: " (" attr(href) ")"; }
  abbr[title]::after { content: " (" attr(title) ")"; }
  a[href^=3D"#"]::after, a[href^=3D"javascript:"]::after { content: ""; }
  pre, blockquote { border: 1px solid rgb(153, 153, 153); break-inside: avo=
id; }
  thead { display: table-header-group; }
  tr, img { break-inside: avoid; }
  img { max-width: 100% !important; }
  p, h2, h3 { orphans: 3; widows: 3; }
  h2, h3 { break-after: avoid; }
  .navbar { display: none; }
  .btn > .caret, .dropup > .btn > .caret { border-top-color: rgb(0, 0, 0) !=
important; }
  .label { border: 1px solid rgb(0, 0, 0); }
  .table { border-collapse: collapse !important; }
  .table td, .table th { background-color: rgb(255, 255, 255) !important; }
  .table-bordered th, .table-bordered td { border: 1px solid rgb(221, 221, =
221) !important; }
}

@font-face { font-family: "Glyphicons Halflings"; src: url("../components/b=
ootstrap/fonts/glyphicons-halflings-regular.woff2") format("woff2"), url(".=
./components/bootstrap/fonts/glyphicons-halflings-regular.woff") format("wo=
ff"), url("../components/bootstrap/fonts/glyphicons-halflings-regular.ttf")=
 format("truetype"); }

.glyphicon { position: relative; top: 1px; display: inline-block; font-fami=
ly: "Glyphicons Halflings"; font-style: normal; font-weight: 400; line-heig=
ht: 1; -webkit-font-smoothing: antialiased; }

.glyphicon-asterisk::before { content: "*"; }

.glyphicon-plus::before { content: "+"; }

.glyphicon-euro::before, .glyphicon-eur::before { content: "=E2=82=AC"; }

.glyphicon-minus::before { content: "=E2=88=92"; }

.glyphicon-cloud::before { content: "=E2=98=81"; }

.glyphicon-envelope::before { content: "=E2=9C=89"; }

.glyphicon-pencil::before { content: "=E2=9C=8F"; }

.glyphicon-glass::before { content: "=EE=80=81"; }

.glyphicon-music::before { content: "=EE=80=82"; }

.glyphicon-search::before { content: "=EE=80=83"; }

.glyphicon-heart::before { content: "=EE=80=85"; }

.glyphicon-star::before { content: "=EE=80=86"; }

.glyphicon-star-empty::before { content: "=EE=80=87"; }

.glyphicon-user::before { content: "=EE=80=88"; }

.glyphicon-film::before { content: "=EE=80=89"; }

.glyphicon-th-large::before { content: "=EE=80=90"; }

.glyphicon-th::before { content: "=EE=80=91"; }

.glyphicon-th-list::before { content: "=EE=80=92"; }

.glyphicon-ok::before { content: "=EE=80=93"; }

.glyphicon-remove::before { content: "=EE=80=94"; }

.glyphicon-zoom-in::before { content: "=EE=80=95"; }

.glyphicon-zoom-out::before { content: "=EE=80=96"; }

.glyphicon-off::before { content: "=EE=80=97"; }

.glyphicon-signal::before { content: "=EE=80=98"; }

.glyphicon-cog::before { content: "=EE=80=99"; }

.glyphicon-trash::before { content: "=EE=80=A0"; }

.glyphicon-home::before { content: "=EE=80=A1"; }

.glyphicon-file::before { content: "=EE=80=A2"; }

.glyphicon-time::before { content: "=EE=80=A3"; }

.glyphicon-road::before { content: "=EE=80=A4"; }

.glyphicon-download-alt::before { content: "=EE=80=A5"; }

.glyphicon-download::before { content: "=EE=80=A6"; }

.glyphicon-upload::before { content: "=EE=80=A7"; }

.glyphicon-inbox::before { content: "=EE=80=A8"; }

.glyphicon-play-circle::before { content: "=EE=80=A9"; }

.glyphicon-repeat::before { content: "=EE=80=B0"; }

.glyphicon-refresh::before { content: "=EE=80=B1"; }

.glyphicon-list-alt::before { content: "=EE=80=B2"; }

.glyphicon-lock::before { content: "=EE=80=B3"; }

.glyphicon-flag::before { content: "=EE=80=B4"; }

.glyphicon-headphones::before { content: "=EE=80=B5"; }

.glyphicon-volume-off::before { content: "=EE=80=B6"; }

.glyphicon-volume-down::before { content: "=EE=80=B7"; }

.glyphicon-volume-up::before { content: "=EE=80=B8"; }

.glyphicon-qrcode::before { content: "=EE=80=B9"; }

.glyphicon-barcode::before { content: "=EE=81=80"; }

.glyphicon-tag::before { content: "=EE=81=81"; }

.glyphicon-tags::before { content: "=EE=81=82"; }

.glyphicon-book::before { content: "=EE=81=83"; }

.glyphicon-bookmark::before { content: "=EE=81=84"; }

.glyphicon-print::before { content: "=EE=81=85"; }

.glyphicon-camera::before { content: "=EE=81=86"; }

.glyphicon-font::before { content: "=EE=81=87"; }

.glyphicon-bold::before { content: "=EE=81=88"; }

.glyphicon-italic::before { content: "=EE=81=89"; }

.glyphicon-text-height::before { content: "=EE=81=90"; }

.glyphicon-text-width::before { content: "=EE=81=91"; }

.glyphicon-align-left::before { content: "=EE=81=92"; }

.glyphicon-align-center::before { content: "=EE=81=93"; }

.glyphicon-align-right::before { content: "=EE=81=94"; }

.glyphicon-align-justify::before { content: "=EE=81=95"; }

.glyphicon-list::before { content: "=EE=81=96"; }

.glyphicon-indent-left::before { content: "=EE=81=97"; }

.glyphicon-indent-right::before { content: "=EE=81=98"; }

.glyphicon-facetime-video::before { content: "=EE=81=99"; }

.glyphicon-picture::before { content: "=EE=81=A0"; }

.glyphicon-map-marker::before { content: "=EE=81=A2"; }

.glyphicon-adjust::before { content: "=EE=81=A3"; }

.glyphicon-tint::before { content: "=EE=81=A4"; }

.glyphicon-edit::before { content: "=EE=81=A5"; }

.glyphicon-share::before { content: "=EE=81=A6"; }

.glyphicon-check::before { content: "=EE=81=A7"; }

.glyphicon-move::before { content: "=EE=81=A8"; }

.glyphicon-step-backward::before { content: "=EE=81=A9"; }

.glyphicon-fast-backward::before { content: "=EE=81=B0"; }

.glyphicon-backward::before { content: "=EE=81=B1"; }

.glyphicon-play::before { content: "=EE=81=B2"; }

.glyphicon-pause::before { content: "=EE=81=B3"; }

.glyphicon-stop::before { content: "=EE=81=B4"; }

.glyphicon-forward::before { content: "=EE=81=B5"; }

.glyphicon-fast-forward::before { content: "=EE=81=B6"; }

.glyphicon-step-forward::before { content: "=EE=81=B7"; }

.glyphicon-eject::before { content: "=EE=81=B8"; }

.glyphicon-chevron-left::before { content: "=EE=81=B9"; }

.glyphicon-chevron-right::before { content: "=EE=82=80"; }

.glyphicon-plus-sign::before { content: "=EE=82=81"; }

.glyphicon-minus-sign::before { content: "=EE=82=82"; }

.glyphicon-remove-sign::before { content: "=EE=82=83"; }

.glyphicon-ok-sign::before { content: "=EE=82=84"; }

.glyphicon-question-sign::before { content: "=EE=82=85"; }

.glyphicon-info-sign::before { content: "=EE=82=86"; }

.glyphicon-screenshot::before { content: "=EE=82=87"; }

.glyphicon-remove-circle::before { content: "=EE=82=88"; }

.glyphicon-ok-circle::before { content: "=EE=82=89"; }

.glyphicon-ban-circle::before { content: "=EE=82=90"; }

.glyphicon-arrow-left::before { content: "=EE=82=91"; }

.glyphicon-arrow-right::before { content: "=EE=82=92"; }

.glyphicon-arrow-up::before { content: "=EE=82=93"; }

.glyphicon-arrow-down::before { content: "=EE=82=94"; }

.glyphicon-share-alt::before { content: "=EE=82=95"; }

.glyphicon-resize-full::before { content: "=EE=82=96"; }

.glyphicon-resize-small::before { content: "=EE=82=97"; }

.glyphicon-exclamation-sign::before { content: "=EE=84=81"; }

.glyphicon-gift::before { content: "=EE=84=82"; }

.glyphicon-leaf::before { content: "=EE=84=83"; }

.glyphicon-fire::before { content: "=EE=84=84"; }

.glyphicon-eye-open::before { content: "=EE=84=85"; }

.glyphicon-eye-close::before { content: "=EE=84=86"; }

.glyphicon-warning-sign::before { content: "=EE=84=87"; }

.glyphicon-plane::before { content: "=EE=84=88"; }

.glyphicon-calendar::before { content: "=EE=84=89"; }

.glyphicon-random::before { content: "=EE=84=90"; }

.glyphicon-comment::before { content: "=EE=84=91"; }

.glyphicon-magnet::before { content: "=EE=84=92"; }

.glyphicon-chevron-up::before { content: "=EE=84=93"; }

.glyphicon-chevron-down::before { content: "=EE=84=94"; }

.glyphicon-retweet::before { content: "=EE=84=95"; }

.glyphicon-shopping-cart::before { content: "=EE=84=96"; }

.glyphicon-folder-close::before { content: "=EE=84=97"; }

.glyphicon-folder-open::before { content: "=EE=84=98"; }

.glyphicon-resize-vertical::before { content: "=EE=84=99"; }

.glyphicon-resize-horizontal::before { content: "=EE=84=A0"; }

.glyphicon-hdd::before { content: "=EE=84=A1"; }

.glyphicon-bullhorn::before { content: "=EE=84=A2"; }

.glyphicon-bell::before { content: "=EE=84=A3"; }

.glyphicon-certificate::before { content: "=EE=84=A4"; }

.glyphicon-thumbs-up::before { content: "=EE=84=A5"; }

.glyphicon-thumbs-down::before { content: "=EE=84=A6"; }

.glyphicon-hand-right::before { content: "=EE=84=A7"; }

.glyphicon-hand-left::before { content: "=EE=84=A8"; }

.glyphicon-hand-up::before { content: "=EE=84=A9"; }

.glyphicon-hand-down::before { content: "=EE=84=B0"; }

.glyphicon-circle-arrow-right::before { content: "=EE=84=B1"; }

.glyphicon-circle-arrow-left::before { content: "=EE=84=B2"; }

.glyphicon-circle-arrow-up::before { content: "=EE=84=B3"; }

.glyphicon-circle-arrow-down::before { content: "=EE=84=B4"; }

.glyphicon-globe::before { content: "=EE=84=B5"; }

.glyphicon-wrench::before { content: "=EE=84=B6"; }

.glyphicon-tasks::before { content: "=EE=84=B7"; }

.glyphicon-filter::before { content: "=EE=84=B8"; }

.glyphicon-briefcase::before { content: "=EE=84=B9"; }

.glyphicon-fullscreen::before { content: "=EE=85=80"; }

.glyphicon-dashboard::before { content: "=EE=85=81"; }

.glyphicon-paperclip::before { content: "=EE=85=82"; }

.glyphicon-heart-empty::before { content: "=EE=85=83"; }

.glyphicon-link::before { content: "=EE=85=84"; }

.glyphicon-phone::before { content: "=EE=85=85"; }

.glyphicon-pushpin::before { content: "=EE=85=86"; }

.glyphicon-usd::before { content: "=EE=85=88"; }

.glyphicon-gbp::before { content: "=EE=85=89"; }

.glyphicon-sort::before { content: "=EE=85=90"; }

.glyphicon-sort-by-alphabet::before { content: "=EE=85=91"; }

.glyphicon-sort-by-alphabet-alt::before { content: "=EE=85=92"; }

.glyphicon-sort-by-order::before { content: "=EE=85=93"; }

.glyphicon-sort-by-order-alt::before { content: "=EE=85=94"; }

.glyphicon-sort-by-attributes::before { content: "=EE=85=95"; }

.glyphicon-sort-by-attributes-alt::before { content: "=EE=85=96"; }

.glyphicon-unchecked::before { content: "=EE=85=97"; }

.glyphicon-expand::before { content: "=EE=85=98"; }

.glyphicon-collapse-down::before { content: "=EE=85=99"; }

.glyphicon-collapse-up::before { content: "=EE=85=A0"; }

.glyphicon-log-in::before { content: "=EE=85=A1"; }

.glyphicon-flash::before { content: "=EE=85=A2"; }

.glyphicon-log-out::before { content: "=EE=85=A3"; }

.glyphicon-new-window::before { content: "=EE=85=A4"; }

.glyphicon-record::before { content: "=EE=85=A5"; }

.glyphicon-save::before { content: "=EE=85=A6"; }

.glyphicon-open::before { content: "=EE=85=A7"; }

.glyphicon-saved::before { content: "=EE=85=A8"; }

.glyphicon-import::before { content: "=EE=85=A9"; }

.glyphicon-export::before { content: "=EE=85=B0"; }

.glyphicon-send::before { content: "=EE=85=B1"; }

.glyphicon-floppy-disk::before { content: "=EE=85=B2"; }

.glyphicon-floppy-saved::before { content: "=EE=85=B3"; }

.glyphicon-floppy-remove::before { content: "=EE=85=B4"; }

.glyphicon-floppy-save::before { content: "=EE=85=B5"; }

.glyphicon-floppy-open::before { content: "=EE=85=B6"; }

.glyphicon-credit-card::before { content: "=EE=85=B7"; }

.glyphicon-transfer::before { content: "=EE=85=B8"; }

.glyphicon-cutlery::before { content: "=EE=85=B9"; }

.glyphicon-header::before { content: "=EE=86=80"; }

.glyphicon-compressed::before { content: "=EE=86=81"; }

.glyphicon-earphone::before { content: "=EE=86=82"; }

.glyphicon-phone-alt::before { content: "=EE=86=83"; }

.glyphicon-tower::before { content: "=EE=86=84"; }

.glyphicon-stats::before { content: "=EE=86=85"; }

.glyphicon-sd-video::before { content: "=EE=86=86"; }

.glyphicon-hd-video::before { content: "=EE=86=87"; }

.glyphicon-subtitles::before { content: "=EE=86=88"; }

.glyphicon-sound-stereo::before { content: "=EE=86=89"; }

.glyphicon-sound-dolby::before { content: "=EE=86=90"; }

.glyphicon-sound-5-1::before { content: "=EE=86=91"; }

.glyphicon-sound-6-1::before { content: "=EE=86=92"; }

.glyphicon-sound-7-1::before { content: "=EE=86=93"; }

.glyphicon-copyright-mark::before { content: "=EE=86=94"; }

.glyphicon-registration-mark::before { content: "=EE=86=95"; }

.glyphicon-cloud-download::before { content: "=EE=86=97"; }

.glyphicon-cloud-upload::before { content: "=EE=86=98"; }

.glyphicon-tree-conifer::before { content: "=EE=86=99"; }

.glyphicon-tree-deciduous::before { content: "=EE=88=80"; }

.glyphicon-cd::before { content: "=EE=88=81"; }

.glyphicon-save-file::before { content: "=EE=88=82"; }

.glyphicon-open-file::before { content: "=EE=88=83"; }

.glyphicon-level-up::before { content: "=EE=88=84"; }

.glyphicon-copy::before { content: "=EE=88=85"; }

.glyphicon-paste::before { content: "=EE=88=86"; }

.glyphicon-alert::before { content: "=EE=88=89"; }

.glyphicon-equalizer::before { content: "=EE=88=90"; }

.glyphicon-king::before { content: "=EE=88=91"; }

.glyphicon-queen::before { content: "=EE=88=92"; }

.glyphicon-pawn::before { content: "=EE=88=93"; }

.glyphicon-bishop::before { content: "=EE=88=94"; }

.glyphicon-knight::before { content: "=EE=88=95"; }

.glyphicon-baby-formula::before { content: "=EE=88=96"; }

.glyphicon-tent::before { content: "=E2=9B=BA"; }

.glyphicon-blackboard::before { content: "=EE=88=98"; }

.glyphicon-bed::before { content: "=EE=88=99"; }

.glyphicon-apple::before { content: "=EF=A3=BF"; }

.glyphicon-erase::before { content: "=EE=88=A1"; }

.glyphicon-hourglass::before { content: "=E2=8C=9B"; }

.glyphicon-lamp::before { content: "=EE=88=A3"; }

.glyphicon-duplicate::before { content: "=EE=88=A4"; }

.glyphicon-piggy-bank::before { content: "=EE=88=A5"; }

.glyphicon-scissors::before { content: "=EE=88=A6"; }

.glyphicon-bitcoin::before { content: "=EE=88=A7"; }

.glyphicon-btc::before { content: "=EE=88=A7"; }

.glyphicon-xbt::before { content: "=EE=88=A7"; }

.glyphicon-yen::before { content: "=C2=A5"; }

.glyphicon-jpy::before { content: "=C2=A5"; }

.glyphicon-ruble::before { content: "=E2=82=BD"; }

.glyphicon-rub::before { content: "=E2=82=BD"; }

.glyphicon-scale::before { content: "=EE=88=B0"; }

.glyphicon-ice-lolly::before { content: "=EE=88=B1"; }

.glyphicon-ice-lolly-tasted::before { content: "=EE=88=B2"; }

.glyphicon-education::before { content: "=EE=88=B3"; }

.glyphicon-option-horizontal::before { content: "=EE=88=B4"; }

.glyphicon-option-vertical::before { content: "=EE=88=B5"; }

.glyphicon-menu-hamburger::before { content: "=EE=88=B6"; }

.glyphicon-modal-window::before { content: "=EE=88=B7"; }

.glyphicon-oil::before { content: "=EE=88=B8"; }

.glyphicon-grain::before { content: "=EE=88=B9"; }

.glyphicon-sunglasses::before { content: "=EE=89=80"; }

.glyphicon-text-size::before { content: "=EE=89=81"; }

.glyphicon-text-color::before { content: "=EE=89=82"; }

.glyphicon-text-background::before { content: "=EE=89=83"; }

.glyphicon-object-align-top::before { content: "=EE=89=84"; }

.glyphicon-object-align-bottom::before { content: "=EE=89=85"; }

.glyphicon-object-align-horizontal::before { content: "=EE=89=86"; }

.glyphicon-object-align-left::before { content: "=EE=89=87"; }

.glyphicon-object-align-vertical::before { content: "=EE=89=88"; }

.glyphicon-object-align-right::before { content: "=EE=89=89"; }

.glyphicon-triangle-right::before { content: "=EE=89=90"; }

.glyphicon-triangle-left::before { content: "=EE=89=91"; }

.glyphicon-triangle-bottom::before { content: "=EE=89=92"; }

.glyphicon-triangle-top::before { content: "=EE=89=93"; }

.glyphicon-console::before { content: "=EE=89=94"; }

.glyphicon-superscript::before { content: "=EE=89=95"; }

.glyphicon-subscript::before { content: "=EE=89=96"; }

.glyphicon-menu-left::before { content: "=EE=89=97"; }

.glyphicon-menu-right::before { content: "=EE=89=98"; }

.glyphicon-menu-down::before { content: "=EE=89=99"; }

.glyphicon-menu-up::before { content: "=EE=89=A0"; }

* { box-sizing: border-box; }

::before, ::after { box-sizing: border-box; }

html { font-size: 10px; -webkit-tap-highlight-color: rgba(0, 0, 0, 0); }

body { font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; font-si=
ze: 13px; line-height: 1.42857; color: rgb(0, 0, 0); background-color: rgb(=
255, 255, 255); }

input, button, select, textarea { font-family: inherit; font-size: inherit;=
 line-height: inherit; }

a { color: rgb(41, 110, 170); text-decoration: none; }

a:hover, a:focus { color: rgb(26, 70, 108); text-decoration: underline; }

a:focus { outline: -webkit-focus-ring-color auto 5px; outline-offset: -2px;=
 }

figure { margin: 0px; }

img { vertical-align: middle; }

.img-responsive, .thumbnail > img, .thumbnail a > img, .carousel-inner > .i=
tem > img, .carousel-inner > .item > a > img { display: block; max-width: 1=
00%; height: auto; }

.img-rounded { border-radius: 3px; }

.img-thumbnail { padding: 4px; line-height: 1.42857; background-color: rgb(=
255, 255, 255); border: 1px solid rgb(221, 221, 221); border-radius: 2px; t=
ransition: all 0.2s ease-in-out 0s; display: inline-block; max-width: 100%;=
 height: auto; }

.img-circle { border-radius: 50%; }

hr { margin-top: 18px; margin-bottom: 18px; border-width: 1px 0px 0px; bord=
er-right-style: initial; border-bottom-style: initial; border-left-style: i=
nitial; border-right-color: initial; border-bottom-color: initial; border-l=
eft-color: initial; border-image: initial; border-top-style: solid; border-=
top-color: rgb(238, 238, 238); }

.sr-only { position: absolute; width: 1px; height: 1px; padding: 0px; margi=
n: -1px; overflow: hidden; clip: rect(0px, 0px, 0px, 0px); border: 0px; }

.sr-only-focusable:active, .sr-only-focusable:focus { position: static; wid=
th: auto; height: auto; margin: 0px; overflow: visible; clip: auto; }

[role=3D"button"] { cursor: pointer; }

h1, h2, h3, h4, h5, h6, .h1, .h2, .h3, .h4, .h5, .h6 { font-family: inherit=
; font-weight: 500; line-height: 1.1; color: inherit; }

h1 small, h2 small, h3 small, h4 small, h5 small, h6 small, .h1 small, .h2 =
small, .h3 small, .h4 small, .h5 small, .h6 small, h1 .small, h2 .small, h3=
 .small, h4 .small, h5 .small, h6 .small, .h1 .small, .h2 .small, .h3 .smal=
l, .h4 .small, .h5 .small, .h6 .small { font-weight: 400; line-height: 1; c=
olor: rgb(119, 119, 119); }

h1, .h1, h2, .h2, h3, .h3 { margin-top: 18px; margin-bottom: 9px; }

h1 small, .h1 small, h2 small, .h2 small, h3 small, .h3 small, h1 .small, .=
h1 .small, h2 .small, .h2 .small, h3 .small, .h3 .small { font-size: 65%; }

h4, .h4, h5, .h5, h6, .h6 { margin-top: 9px; margin-bottom: 9px; }

h4 small, .h4 small, h5 small, .h5 small, h6 small, .h6 small, h4 .small, .=
h4 .small, h5 .small, .h5 .small, h6 .small, .h6 .small { font-size: 75%; }

h1, .h1 { font-size: 33px; }

h2, .h2 { font-size: 27px; }

h3, .h3 { font-size: 23px; }

h4, .h4 { font-size: 17px; }

h5, .h5 { font-size: 13px; }

h6, .h6 { font-size: 12px; }

p { margin: 0px 0px 9px; }

.lead { margin-bottom: 18px; font-size: 14px; font-weight: 300; line-height=
: 1.4; }

@media (min-width: 768px) {
  .lead { font-size: 19.5px; }
}

small, .small { font-size: 92%; }

mark, .mark { padding: 0.2em; background-color: rgb(252, 248, 227); }

.text-left { text-align: left; }

.text-right { text-align: right; }

.text-center { text-align: center; }

.text-justify { text-align: justify; }

.text-nowrap { white-space: nowrap; }

.text-lowercase { text-transform: lowercase; }

.text-uppercase { text-transform: uppercase; }

.text-capitalize { text-transform: capitalize; }

.text-muted { color: rgb(119, 119, 119); }

.text-primary { color: rgb(51, 122, 183); }

a.text-primary:hover, a.text-primary:focus { color: rgb(40, 96, 144); }

.text-success { color: rgb(60, 118, 61); }

a.text-success:hover, a.text-success:focus { color: rgb(43, 84, 44); }

.text-info { color: rgb(49, 112, 143); }

a.text-info:hover, a.text-info:focus { color: rgb(36, 82, 105); }

.text-warning { color: rgb(138, 109, 59); }

a.text-warning:hover, a.text-warning:focus { color: rgb(102, 81, 44); }

.text-danger { color: rgb(169, 68, 66); }

a.text-danger:hover, a.text-danger:focus { color: rgb(132, 53, 52); }

.bg-primary { color: rgb(255, 255, 255); background-color: rgb(51, 122, 183=
); }

a.bg-primary:hover, a.bg-primary:focus { background-color: rgb(40, 96, 144)=
; }

.bg-success { background-color: rgb(223, 240, 216); }

a.bg-success:hover, a.bg-success:focus { background-color: rgb(193, 226, 17=
9); }

.bg-info { background-color: rgb(217, 237, 247); }

a.bg-info:hover, a.bg-info:focus { background-color: rgb(175, 217, 238); }

.bg-warning { background-color: rgb(252, 248, 227); }

a.bg-warning:hover, a.bg-warning:focus { background-color: rgb(247, 236, 18=
1); }

.bg-danger { background-color: rgb(242, 222, 222); }

a.bg-danger:hover, a.bg-danger:focus { background-color: rgb(228, 185, 185)=
; }

.page-header { padding-bottom: 8px; margin: 36px 0px 18px; border-bottom: 1=
px solid rgb(238, 238, 238); }

ul, ol { margin-top: 0px; margin-bottom: 9px; }

ul ul, ol ul, ul ol, ol ol { margin-bottom: 0px; }

.list-unstyled { padding-left: 0px; list-style: none; }

.list-inline { padding-left: 0px; list-style: none; margin-left: -5px; }

.list-inline > li { display: inline-block; padding-right: 5px; padding-left=
: 5px; }

dl { margin-top: 0px; margin-bottom: 18px; }

dt, dd { line-height: 1.42857; }

dt { font-weight: 700; }

dd { margin-left: 0px; }

@media (min-width: 541px) {
  .dl-horizontal dt { float: left; width: 160px; clear: left; text-align: r=
ight; overflow: hidden; text-overflow: ellipsis; white-space: nowrap; }
  .dl-horizontal dd { margin-left: 180px; }
}

abbr[title], abbr[data-original-title] { cursor: help; }

.initialism { font-size: 90%; text-transform: uppercase; }

blockquote { padding: 9px 18px; margin: 0px 0px 18px; font-size: inherit; b=
order-left: 5px solid rgb(238, 238, 238); }

blockquote p:last-child, blockquote ul:last-child, blockquote ol:last-child=
 { margin-bottom: 0px; }

blockquote footer, blockquote small, blockquote .small { display: block; fo=
nt-size: 80%; line-height: 1.42857; color: rgb(119, 119, 119); }

blockquote footer::before, blockquote small::before, blockquote .small::bef=
ore { content: "=E2=80=94=C2=A0"; }

.blockquote-reverse, blockquote.pull-right { padding-right: 15px; padding-l=
eft: 0px; text-align: right; border-right: 5px solid rgb(238, 238, 238); bo=
rder-left: 0px; }

.blockquote-reverse footer::before, blockquote.pull-right footer::before, .=
blockquote-reverse small::before, blockquote.pull-right small::before, .blo=
ckquote-reverse .small::before, blockquote.pull-right .small::before { cont=
ent: ""; }

.blockquote-reverse footer::after, blockquote.pull-right footer::after, .bl=
ockquote-reverse small::after, blockquote.pull-right small::after, .blockqu=
ote-reverse .small::after, blockquote.pull-right .small::after { content: "=
=C2=A0=E2=80=94"; }

address { margin-bottom: 18px; font-style: normal; line-height: 1.42857; }

code, kbd, pre, samp { font-family: monospace; }

code { padding: 2px 4px; font-size: 90%; color: rgb(199, 37, 78); backgroun=
d-color: rgb(249, 242, 244); border-radius: 2px; }

kbd { padding: 2px 4px; font-size: 90%; color: rgb(136, 136, 136); backgrou=
nd-color: transparent; border-radius: 1px; box-shadow: rgba(0, 0, 0, 0.25) =
0px -1px 0px inset; }

kbd kbd { padding: 0px; font-size: 100%; font-weight: 700; box-shadow: none=
; }

pre { display: block; padding: 8.5px; margin: 0px 0px 9px; font-size: 12px;=
 line-height: 1.42857; color: rgb(51, 51, 51); word-break: break-all; overf=
low-wrap: break-word; background-color: rgb(245, 245, 245); border: 1px sol=
id rgb(204, 204, 204); border-radius: 2px; }

pre code { padding: 0px; font-size: inherit; color: inherit; white-space: p=
re-wrap; background-color: transparent; border-radius: 0px; }

.pre-scrollable { max-height: 340px; overflow-y: scroll; }

.container { padding-right: 0px; padding-left: 0px; margin-right: auto; mar=
gin-left: auto; }

@media (min-width: 768px) {
  .container { width: 768px; }
}

@media (min-width: 992px) {
  .container { width: 940px; }
}

@media (min-width: 1200px) {
  .container { width: 1140px; }
}

.container-fluid { padding-right: 0px; padding-left: 0px; margin-right: aut=
o; margin-left: auto; }

.row { margin-right: 0px; margin-left: 0px; }

.row-no-gutters { margin-right: 0px; margin-left: 0px; }

.row-no-gutters [class*=3D"col-"] { padding-right: 0px; padding-left: 0px; =
}

.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2=
, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm=
-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-=
xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .co=
l-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .=
col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-x=
s-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-1=
2, .col-lg-12 { position: relative; min-height: 1px; padding-right: 0px; pa=
dding-left: 0px; }

.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7=
, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 { float: left; }

.col-xs-12 { width: 100%; }

.col-xs-11 { width: 91.6667%; }

.col-xs-10 { width: 83.3333%; }

.col-xs-9 { width: 75%; }

.col-xs-8 { width: 66.6667%; }

.col-xs-7 { width: 58.3333%; }

.col-xs-6 { width: 50%; }

.col-xs-5 { width: 41.6667%; }

.col-xs-4 { width: 33.3333%; }

.col-xs-3 { width: 25%; }

.col-xs-2 { width: 16.6667%; }

.col-xs-1 { width: 8.33333%; }

.col-xs-pull-12 { right: 100%; }

.col-xs-pull-11 { right: 91.6667%; }

.col-xs-pull-10 { right: 83.3333%; }

.col-xs-pull-9 { right: 75%; }

.col-xs-pull-8 { right: 66.6667%; }

.col-xs-pull-7 { right: 58.3333%; }

.col-xs-pull-6 { right: 50%; }

.col-xs-pull-5 { right: 41.6667%; }

.col-xs-pull-4 { right: 33.3333%; }

.col-xs-pull-3 { right: 25%; }

.col-xs-pull-2 { right: 16.6667%; }

.col-xs-pull-1 { right: 8.33333%; }

.col-xs-pull-0 { right: auto; }

.col-xs-push-12 { left: 100%; }

.col-xs-push-11 { left: 91.6667%; }

.col-xs-push-10 { left: 83.3333%; }

.col-xs-push-9 { left: 75%; }

.col-xs-push-8 { left: 66.6667%; }

.col-xs-push-7 { left: 58.3333%; }

.col-xs-push-6 { left: 50%; }

.col-xs-push-5 { left: 41.6667%; }

.col-xs-push-4 { left: 33.3333%; }

.col-xs-push-3 { left: 25%; }

.col-xs-push-2 { left: 16.6667%; }

.col-xs-push-1 { left: 8.33333%; }

.col-xs-push-0 { left: auto; }

.col-xs-offset-12 { margin-left: 100%; }

.col-xs-offset-11 { margin-left: 91.6667%; }

.col-xs-offset-10 { margin-left: 83.3333%; }

.col-xs-offset-9 { margin-left: 75%; }

.col-xs-offset-8 { margin-left: 66.6667%; }

.col-xs-offset-7 { margin-left: 58.3333%; }

.col-xs-offset-6 { margin-left: 50%; }

.col-xs-offset-5 { margin-left: 41.6667%; }

.col-xs-offset-4 { margin-left: 33.3333%; }

.col-xs-offset-3 { margin-left: 25%; }

.col-xs-offset-2 { margin-left: 16.6667%; }

.col-xs-offset-1 { margin-left: 8.33333%; }

.col-xs-offset-0 { margin-left: 0%; }

@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm=
-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 { float: left;=
 }
  .col-sm-12 { width: 100%; }
  .col-sm-11 { width: 91.6667%; }
  .col-sm-10 { width: 83.3333%; }
  .col-sm-9 { width: 75%; }
  .col-sm-8 { width: 66.6667%; }
  .col-sm-7 { width: 58.3333%; }
  .col-sm-6 { width: 50%; }
  .col-sm-5 { width: 41.6667%; }
  .col-sm-4 { width: 33.3333%; }
  .col-sm-3 { width: 25%; }
  .col-sm-2 { width: 16.6667%; }
  .col-sm-1 { width: 8.33333%; }
  .col-sm-pull-12 { right: 100%; }
  .col-sm-pull-11 { right: 91.6667%; }
  .col-sm-pull-10 { right: 83.3333%; }
  .col-sm-pull-9 { right: 75%; }
  .col-sm-pull-8 { right: 66.6667%; }
  .col-sm-pull-7 { right: 58.3333%; }
  .col-sm-pull-6 { right: 50%; }
  .col-sm-pull-5 { right: 41.6667%; }
  .col-sm-pull-4 { right: 33.3333%; }
  .col-sm-pull-3 { right: 25%; }
  .col-sm-pull-2 { right: 16.6667%; }
  .col-sm-pull-1 { right: 8.33333%; }
  .col-sm-pull-0 { right: auto; }
  .col-sm-push-12 { left: 100%; }
  .col-sm-push-11 { left: 91.6667%; }
  .col-sm-push-10 { left: 83.3333%; }
  .col-sm-push-9 { left: 75%; }
  .col-sm-push-8 { left: 66.6667%; }
  .col-sm-push-7 { left: 58.3333%; }
  .col-sm-push-6 { left: 50%; }
  .col-sm-push-5 { left: 41.6667%; }
  .col-sm-push-4 { left: 33.3333%; }
  .col-sm-push-3 { left: 25%; }
  .col-sm-push-2 { left: 16.6667%; }
  .col-sm-push-1 { left: 8.33333%; }
  .col-sm-push-0 { left: auto; }
  .col-sm-offset-12 { margin-left: 100%; }
  .col-sm-offset-11 { margin-left: 91.6667%; }
  .col-sm-offset-10 { margin-left: 83.3333%; }
  .col-sm-offset-9 { margin-left: 75%; }
  .col-sm-offset-8 { margin-left: 66.6667%; }
  .col-sm-offset-7 { margin-left: 58.3333%; }
  .col-sm-offset-6 { margin-left: 50%; }
  .col-sm-offset-5 { margin-left: 41.6667%; }
  .col-sm-offset-4 { margin-left: 33.3333%; }
  .col-sm-offset-3 { margin-left: 25%; }
  .col-sm-offset-2 { margin-left: 16.6667%; }
  .col-sm-offset-1 { margin-left: 8.33333%; }
  .col-sm-offset-0 { margin-left: 0%; }
}

@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md=
-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 { float: left;=
 }
  .col-md-12 { width: 100%; }
  .col-md-11 { width: 91.6667%; }
  .col-md-10 { width: 83.3333%; }
  .col-md-9 { width: 75%; }
  .col-md-8 { width: 66.6667%; }
  .col-md-7 { width: 58.3333%; }
  .col-md-6 { width: 50%; }
  .col-md-5 { width: 41.6667%; }
  .col-md-4 { width: 33.3333%; }
  .col-md-3 { width: 25%; }
  .col-md-2 { width: 16.6667%; }
  .col-md-1 { width: 8.33333%; }
  .col-md-pull-12 { right: 100%; }
  .col-md-pull-11 { right: 91.6667%; }
  .col-md-pull-10 { right: 83.3333%; }
  .col-md-pull-9 { right: 75%; }
  .col-md-pull-8 { right: 66.6667%; }
  .col-md-pull-7 { right: 58.3333%; }
  .col-md-pull-6 { right: 50%; }
  .col-md-pull-5 { right: 41.6667%; }
  .col-md-pull-4 { right: 33.3333%; }
  .col-md-pull-3 { right: 25%; }
  .col-md-pull-2 { right: 16.6667%; }
  .col-md-pull-1 { right: 8.33333%; }
  .col-md-pull-0 { right: auto; }
  .col-md-push-12 { left: 100%; }
  .col-md-push-11 { left: 91.6667%; }
  .col-md-push-10 { left: 83.3333%; }
  .col-md-push-9 { left: 75%; }
  .col-md-push-8 { left: 66.6667%; }
  .col-md-push-7 { left: 58.3333%; }
  .col-md-push-6 { left: 50%; }
  .col-md-push-5 { left: 41.6667%; }
  .col-md-push-4 { left: 33.3333%; }
  .col-md-push-3 { left: 25%; }
  .col-md-push-2 { left: 16.6667%; }
  .col-md-push-1 { left: 8.33333%; }
  .col-md-push-0 { left: auto; }
  .col-md-offset-12 { margin-left: 100%; }
  .col-md-offset-11 { margin-left: 91.6667%; }
  .col-md-offset-10 { margin-left: 83.3333%; }
  .col-md-offset-9 { margin-left: 75%; }
  .col-md-offset-8 { margin-left: 66.6667%; }
  .col-md-offset-7 { margin-left: 58.3333%; }
  .col-md-offset-6 { margin-left: 50%; }
  .col-md-offset-5 { margin-left: 41.6667%; }
  .col-md-offset-4 { margin-left: 33.3333%; }
  .col-md-offset-3 { margin-left: 25%; }
  .col-md-offset-2 { margin-left: 16.6667%; }
  .col-md-offset-1 { margin-left: 8.33333%; }
  .col-md-offset-0 { margin-left: 0%; }
}

@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg=
-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 { float: left;=
 }
  .col-lg-12 { width: 100%; }
  .col-lg-11 { width: 91.6667%; }
  .col-lg-10 { width: 83.3333%; }
  .col-lg-9 { width: 75%; }
  .col-lg-8 { width: 66.6667%; }
  .col-lg-7 { width: 58.3333%; }
  .col-lg-6 { width: 50%; }
  .col-lg-5 { width: 41.6667%; }
  .col-lg-4 { width: 33.3333%; }
  .col-lg-3 { width: 25%; }
  .col-lg-2 { width: 16.6667%; }
  .col-lg-1 { width: 8.33333%; }
  .col-lg-pull-12 { right: 100%; }
  .col-lg-pull-11 { right: 91.6667%; }
  .col-lg-pull-10 { right: 83.3333%; }
  .col-lg-pull-9 { right: 75%; }
  .col-lg-pull-8 { right: 66.6667%; }
  .col-lg-pull-7 { right: 58.3333%; }
  .col-lg-pull-6 { right: 50%; }
  .col-lg-pull-5 { right: 41.6667%; }
  .col-lg-pull-4 { right: 33.3333%; }
  .col-lg-pull-3 { right: 25%; }
  .col-lg-pull-2 { right: 16.6667%; }
  .col-lg-pull-1 { right: 8.33333%; }
  .col-lg-pull-0 { right: auto; }
  .col-lg-push-12 { left: 100%; }
  .col-lg-push-11 { left: 91.6667%; }
  .col-lg-push-10 { left: 83.3333%; }
  .col-lg-push-9 { left: 75%; }
  .col-lg-push-8 { left: 66.6667%; }
  .col-lg-push-7 { left: 58.3333%; }
  .col-lg-push-6 { left: 50%; }
  .col-lg-push-5 { left: 41.6667%; }
  .col-lg-push-4 { left: 33.3333%; }
  .col-lg-push-3 { left: 25%; }
  .col-lg-push-2 { left: 16.6667%; }
  .col-lg-push-1 { left: 8.33333%; }
  .col-lg-push-0 { left: auto; }
  .col-lg-offset-12 { margin-left: 100%; }
  .col-lg-offset-11 { margin-left: 91.6667%; }
  .col-lg-offset-10 { margin-left: 83.3333%; }
  .col-lg-offset-9 { margin-left: 75%; }
  .col-lg-offset-8 { margin-left: 66.6667%; }
  .col-lg-offset-7 { margin-left: 58.3333%; }
  .col-lg-offset-6 { margin-left: 50%; }
  .col-lg-offset-5 { margin-left: 41.6667%; }
  .col-lg-offset-4 { margin-left: 33.3333%; }
  .col-lg-offset-3 { margin-left: 25%; }
  .col-lg-offset-2 { margin-left: 16.6667%; }
  .col-lg-offset-1 { margin-left: 8.33333%; }
  .col-lg-offset-0 { margin-left: 0%; }
}

table { background-color: transparent; }

table col[class*=3D"col-"] { position: static; display: table-column; float=
: none; }

table td[class*=3D"col-"], table th[class*=3D"col-"] { position: static; di=
splay: table-cell; float: none; }

caption { padding-top: 8px; padding-bottom: 8px; color: rgb(119, 119, 119);=
 text-align: left; }

th { text-align: left; }

.table { width: 100%; max-width: 100%; margin-bottom: 18px; }

.table > thead > tr > th, .table > tbody > tr > th, .table > tfoot > tr > t=
h, .table > thead > tr > td, .table > tbody > tr > td, .table > tfoot > tr =
> td { padding: 8px; line-height: 1.42857; vertical-align: top; border-top:=
 1px solid rgb(221, 221, 221); }

.table > thead > tr > th { vertical-align: bottom; border-bottom: 2px solid=
 rgb(221, 221, 221); }

.table > caption + thead > tr:first-child > th, .table > colgroup + thead >=
 tr:first-child > th, .table > thead:first-child > tr:first-child > th, .ta=
ble > caption + thead > tr:first-child > td, .table > colgroup + thead > tr=
:first-child > td, .table > thead:first-child > tr:first-child > td { borde=
r-top: 0px; }

.table > tbody + tbody { border-top: 2px solid rgb(221, 221, 221); }

.table .table { background-color: rgb(255, 255, 255); }

.table-condensed > thead > tr > th, .table-condensed > tbody > tr > th, .ta=
ble-condensed > tfoot > tr > th, .table-condensed > thead > tr > td, .table=
-condensed > tbody > tr > td, .table-condensed > tfoot > tr > td { padding:=
 5px; }

.table-bordered { border: 1px solid rgb(221, 221, 221); }

.table-bordered > thead > tr > th, .table-bordered > tbody > tr > th, .tabl=
e-bordered > tfoot > tr > th, .table-bordered > thead > tr > td, .table-bor=
dered > tbody > tr > td, .table-bordered > tfoot > tr > td { border: 1px so=
lid rgb(221, 221, 221); }

.table-bordered > thead > tr > th, .table-bordered > thead > tr > td { bord=
er-bottom-width: 2px; }

.table-striped > tbody > tr:nth-of-type(2n+1) { background-color: rgb(249, =
249, 249); }

.table-hover > tbody > tr:hover { background-color: rgb(245, 245, 245); }

.table > thead > tr > td.active, .table > tbody > tr > td.active, .table > =
tfoot > tr > td.active, .table > thead > tr > th.active, .table > tbody > t=
r > th.active, .table > tfoot > tr > th.active, .table > thead > tr.active =
> td, .table > tbody > tr.active > td, .table > tfoot > tr.active > td, .ta=
ble > thead > tr.active > th, .table > tbody > tr.active > th, .table > tfo=
ot > tr.active > th { background-color: rgb(245, 245, 245); }

.table-hover > tbody > tr > td.active:hover, .table-hover > tbody > tr > th=
.active:hover, .table-hover > tbody > tr.active:hover > td, .table-hover > =
tbody > tr:hover > .active, .table-hover > tbody > tr.active:hover > th { b=
ackground-color: rgb(232, 232, 232); }

.table > thead > tr > td.success, .table > tbody > tr > td.success, .table =
> tfoot > tr > td.success, .table > thead > tr > th.success, .table > tbody=
 > tr > th.success, .table > tfoot > tr > th.success, .table > thead > tr.s=
uccess > td, .table > tbody > tr.success > td, .table > tfoot > tr.success =
> td, .table > thead > tr.success > th, .table > tbody > tr.success > th, .=
table > tfoot > tr.success > th { background-color: rgb(223, 240, 216); }

.table-hover > tbody > tr > td.success:hover, .table-hover > tbody > tr > t=
h.success:hover, .table-hover > tbody > tr.success:hover > td, .table-hover=
 > tbody > tr:hover > .success, .table-hover > tbody > tr.success:hover > t=
h { background-color: rgb(208, 233, 198); }

.table > thead > tr > td.info, .table > tbody > tr > td.info, .table > tfoo=
t > tr > td.info, .table > thead > tr > th.info, .table > tbody > tr > th.i=
nfo, .table > tfoot > tr > th.info, .table > thead > tr.info > td, .table >=
 tbody > tr.info > td, .table > tfoot > tr.info > td, .table > thead > tr.i=
nfo > th, .table > tbody > tr.info > th, .table > tfoot > tr.info > th { ba=
ckground-color: rgb(217, 237, 247); }

.table-hover > tbody > tr > td.info:hover, .table-hover > tbody > tr > th.i=
nfo:hover, .table-hover > tbody > tr.info:hover > td, .table-hover > tbody =
> tr:hover > .info, .table-hover > tbody > tr.info:hover > th { background-=
color: rgb(196, 227, 243); }

.table > thead > tr > td.warning, .table > tbody > tr > td.warning, .table =
> tfoot > tr > td.warning, .table > thead > tr > th.warning, .table > tbody=
 > tr > th.warning, .table > tfoot > tr > th.warning, .table > thead > tr.w=
arning > td, .table > tbody > tr.warning > td, .table > tfoot > tr.warning =
> td, .table > thead > tr.warning > th, .table > tbody > tr.warning > th, .=
table > tfoot > tr.warning > th { background-color: rgb(252, 248, 227); }

.table-hover > tbody > tr > td.warning:hover, .table-hover > tbody > tr > t=
h.warning:hover, .table-hover > tbody > tr.warning:hover > td, .table-hover=
 > tbody > tr:hover > .warning, .table-hover > tbody > tr.warning:hover > t=
h { background-color: rgb(250, 242, 204); }

.table > thead > tr > td.danger, .table > tbody > tr > td.danger, .table > =
tfoot > tr > td.danger, .table > thead > tr > th.danger, .table > tbody > t=
r > th.danger, .table > tfoot > tr > th.danger, .table > thead > tr.danger =
> td, .table > tbody > tr.danger > td, .table > tfoot > tr.danger > td, .ta=
ble > thead > tr.danger > th, .table > tbody > tr.danger > th, .table > tfo=
ot > tr.danger > th { background-color: rgb(242, 222, 222); }

.table-hover > tbody > tr > td.danger:hover, .table-hover > tbody > tr > th=
.danger:hover, .table-hover > tbody > tr.danger:hover > td, .table-hover > =
tbody > tr:hover > .danger, .table-hover > tbody > tr.danger:hover > th { b=
ackground-color: rgb(235, 204, 204); }

.table-responsive { min-height: 0.01%; overflow-x: auto; }

@media screen and (max-width: 767px) {
  .table-responsive { width: 100%; margin-bottom: 13.5px; overflow-y: hidde=
n; border: 1px solid rgb(221, 221, 221); }
  .table-responsive > .table { margin-bottom: 0px; }
  .table-responsive > .table > thead > tr > th, .table-responsive > .table =
> tbody > tr > th, .table-responsive > .table > tfoot > tr > th, .table-res=
ponsive > .table > thead > tr > td, .table-responsive > .table > tbody > tr=
 > td, .table-responsive > .table > tfoot > tr > td { white-space: nowrap; =
}
  .table-responsive > .table-bordered { border: 0px; }
  .table-responsive > .table-bordered > thead > tr > th:first-child, .table=
-responsive > .table-bordered > tbody > tr > th:first-child, .table-respons=
ive > .table-bordered > tfoot > tr > th:first-child, .table-responsive > .t=
able-bordered > thead > tr > td:first-child, .table-responsive > .table-bor=
dered > tbody > tr > td:first-child, .table-responsive > .table-bordered > =
tfoot > tr > td:first-child { border-left: 0px; }
  .table-responsive > .table-bordered > thead > tr > th:last-child, .table-=
responsive > .table-bordered > tbody > tr > th:last-child, .table-responsiv=
e > .table-bordered > tfoot > tr > th:last-child, .table-responsive > .tabl=
e-bordered > thead > tr > td:last-child, .table-responsive > .table-bordere=
d > tbody > tr > td:last-child, .table-responsive > .table-bordered > tfoot=
 > tr > td:last-child { border-right: 0px; }
  .table-responsive > .table-bordered > tbody > tr:last-child > th, .table-=
responsive > .table-bordered > tfoot > tr:last-child > th, .table-responsiv=
e > .table-bordered > tbody > tr:last-child > td, .table-responsive > .tabl=
e-bordered > tfoot > tr:last-child > td { border-bottom: 0px; }
}

fieldset { min-width: 0px; padding: 0px; margin: 0px; border: 0px; }

legend { display: block; width: 100%; padding: 0px; margin-bottom: 18px; fo=
nt-size: 19.5px; line-height: inherit; color: rgb(51, 51, 51); border-width=
: 0px 0px 1px; border-top-style: initial; border-right-style: initial; bord=
er-left-style: initial; border-top-color: initial; border-right-color: init=
ial; border-left-color: initial; border-image: initial; border-bottom-style=
: solid; border-bottom-color: rgb(229, 229, 229); }

label { display: inline-block; max-width: 100%; margin-bottom: 5px; font-we=
ight: 700; }

input[type=3D"search"] { box-sizing: border-box; appearance: none; }

input[type=3D"radio"], input[type=3D"checkbox"] { margin: 4px 0px 0px; line=
-height: normal; }

input[type=3D"radio"][disabled], input[type=3D"checkbox"][disabled], input[=
type=3D"radio"].disabled, input[type=3D"checkbox"].disabled, fieldset[disab=
led] input[type=3D"radio"], fieldset[disabled] input[type=3D"checkbox"] { c=
ursor: not-allowed; }

input[type=3D"file"] { display: block; }

input[type=3D"range"] { display: block; width: 100%; }

select[multiple], select[size] { height: auto; }

input[type=3D"file"]:focus, input[type=3D"radio"]:focus, input[type=3D"chec=
kbox"]:focus { outline: -webkit-focus-ring-color auto 5px; outline-offset: =
-2px; }

output { display: block; padding-top: 7px; font-size: 13px; line-height: 1.=
42857; color: rgb(85, 85, 85); }

.form-control { display: block; width: 100%; height: 32px; padding: 6px 12p=
x; font-size: 13px; line-height: 1.42857; color: rgb(85, 85, 85); backgroun=
d-color: rgb(255, 255, 255); background-image: none; border: 1px solid rgb(=
204, 204, 204); border-radius: 2px; box-shadow: rgba(0, 0, 0, 0.075) 0px 1p=
x 1px inset; transition: border-color 0.15s ease-in-out 0s, box-shadow 0.15=
s ease-in-out 0s; }

.form-control:focus { border-color: rgb(102, 175, 233); outline: 0px; box-s=
hadow: rgba(0, 0, 0, 0.075) 0px 1px 1px inset, rgba(102, 175, 233, 0.6) 0px=
 0px 8px; }

.form-control::-webkit-input-placeholder { color: rgb(153, 153, 153); }

.form-control[disabled], .form-control[readonly], fieldset[disabled] .form-=
control { background-color: rgb(238, 238, 238); opacity: 1; }

.form-control[disabled], fieldset[disabled] .form-control { cursor: not-all=
owed; }

textarea.form-control { height: auto; }

@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type=3D"date"].form-control, input[type=3D"time"].form-control, inp=
ut[type=3D"datetime-local"].form-control, input[type=3D"month"].form-contro=
l { line-height: 32px; }
  input[type=3D"date"].input-sm, input[type=3D"time"].input-sm, input[type=
=3D"datetime-local"].input-sm, input[type=3D"month"].input-sm, .input-group=
-sm input[type=3D"date"], .input-group-sm input[type=3D"time"], .input-grou=
p-sm input[type=3D"datetime-local"], .input-group-sm input[type=3D"month"] =
{ line-height: 30px; }
  input[type=3D"date"].input-lg, input[type=3D"time"].input-lg, input[type=
=3D"datetime-local"].input-lg, input[type=3D"month"].input-lg, .input-group=
-lg input[type=3D"date"], .input-group-lg input[type=3D"time"], .input-grou=
p-lg input[type=3D"datetime-local"], .input-group-lg input[type=3D"month"] =
{ line-height: 45px; }
}

.form-group { margin-bottom: 15px; }

.radio, .checkbox { position: relative; display: block; margin-top: 10px; m=
argin-bottom: 10px; }

.radio.disabled label, .checkbox.disabled label, fieldset[disabled] .radio =
label, fieldset[disabled] .checkbox label { cursor: not-allowed; }

.radio label, .checkbox label { min-height: 18px; padding-left: 20px; margi=
n-bottom: 0px; font-weight: 400; cursor: pointer; }

.radio input[type=3D"radio"], .radio-inline input[type=3D"radio"], .checkbo=
x input[type=3D"checkbox"], .checkbox-inline input[type=3D"checkbox"] { pos=
ition: absolute; margin-left: -20px; }

.radio + .radio, .checkbox + .checkbox { margin-top: -5px; }

.radio-inline, .checkbox-inline { position: relative; display: inline-block=
; padding-left: 20px; margin-bottom: 0px; font-weight: 400; vertical-align:=
 middle; cursor: pointer; }

.radio-inline.disabled, .checkbox-inline.disabled, fieldset[disabled] .radi=
o-inline, fieldset[disabled] .checkbox-inline { cursor: not-allowed; }

.radio-inline + .radio-inline, .checkbox-inline + .checkbox-inline { margin=
-top: 0px; margin-left: 10px; }

.form-control-static { min-height: 31px; padding-top: 7px; padding-bottom: =
7px; margin-bottom: 0px; }

.form-control-static.input-lg, .form-control-static.input-sm { padding-righ=
t: 0px; padding-left: 0px; }

.input-sm { height: 30px; padding: 5px 10px; font-size: 12px; line-height: =
1.5; border-radius: 1px; }

select.input-sm { height: 30px; line-height: 30px; }

textarea.input-sm, select[multiple].input-sm { height: auto; }

.form-group-sm .form-control { height: 30px; padding: 5px 10px; font-size: =
12px; line-height: 1.5; border-radius: 1px; }

.form-group-sm select.form-control { height: 30px; line-height: 30px; }

.form-group-sm textarea.form-control, .form-group-sm select[multiple].form-=
control { height: auto; }

.form-group-sm .form-control-static { height: 30px; min-height: 30px; paddi=
ng: 6px 10px; font-size: 12px; line-height: 1.5; }

.input-lg { height: 45px; padding: 10px 16px; font-size: 17px; line-height:=
 1.33333; border-radius: 3px; }

select.input-lg { height: 45px; line-height: 45px; }

textarea.input-lg, select[multiple].input-lg { height: auto; }

.form-group-lg .form-control { height: 45px; padding: 10px 16px; font-size:=
 17px; line-height: 1.33333; border-radius: 3px; }

.form-group-lg select.form-control { height: 45px; line-height: 45px; }

.form-group-lg textarea.form-control, .form-group-lg select[multiple].form-=
control { height: auto; }

.form-group-lg .form-control-static { height: 45px; min-height: 35px; paddi=
ng: 11px 16px; font-size: 17px; line-height: 1.33333; }

.has-feedback { position: relative; }

.has-feedback .form-control { padding-right: 40px; }

.form-control-feedback { position: absolute; top: 0px; right: 0px; z-index:=
 2; display: block; width: 32px; height: 32px; line-height: 32px; text-alig=
n: center; pointer-events: none; }

.input-lg + .form-control-feedback, .input-group-lg + .form-control-feedbac=
k, .form-group-lg .form-control + .form-control-feedback { width: 45px; hei=
ght: 45px; line-height: 45px; }

.input-sm + .form-control-feedback, .input-group-sm + .form-control-feedbac=
k, .form-group-sm .form-control + .form-control-feedback { width: 30px; hei=
ght: 30px; line-height: 30px; }

.has-success .help-block, .has-success .control-label, .has-success .radio,=
 .has-success .checkbox, .has-success .radio-inline, .has-success .checkbox=
-inline, .has-success.radio label, .has-success.checkbox label, .has-succes=
s.radio-inline label, .has-success.checkbox-inline label { color: rgb(60, 1=
18, 61); }

.has-success .form-control { border-color: rgb(60, 118, 61); box-shadow: rg=
ba(0, 0, 0, 0.075) 0px 1px 1px inset; }

.has-success .form-control:focus { border-color: rgb(43, 84, 44); box-shado=
w: rgba(0, 0, 0, 0.075) 0px 1px 1px inset, rgb(103, 177, 104) 0px 0px 6px; =
}

.has-success .input-group-addon { color: rgb(60, 118, 61); background-color=
: rgb(223, 240, 216); border-color: rgb(60, 118, 61); }

.has-success .form-control-feedback { color: rgb(60, 118, 61); }

.has-warning .help-block, .has-warning .control-label, .has-warning .radio,=
 .has-warning .checkbox, .has-warning .radio-inline, .has-warning .checkbox=
-inline, .has-warning.radio label, .has-warning.checkbox label, .has-warnin=
g.radio-inline label, .has-warning.checkbox-inline label { color: rgb(138, =
109, 59); }

.has-warning .form-control { border-color: rgb(138, 109, 59); box-shadow: r=
gba(0, 0, 0, 0.075) 0px 1px 1px inset; }

.has-warning .form-control:focus { border-color: rgb(102, 81, 44); box-shad=
ow: rgba(0, 0, 0, 0.075) 0px 1px 1px inset, rgb(192, 161, 107) 0px 0px 6px;=
 }

.has-warning .input-group-addon { color: rgb(138, 109, 59); background-colo=
r: rgb(252, 248, 227); border-color: rgb(138, 109, 59); }

.has-warning .form-control-feedback { color: rgb(138, 109, 59); }

.has-error .help-block, .has-error .control-label, .has-error .radio, .has-=
error .checkbox, .has-error .radio-inline, .has-error .checkbox-inline, .ha=
s-error.radio label, .has-error.checkbox label, .has-error.radio-inline lab=
el, .has-error.checkbox-inline label { color: rgb(169, 68, 66); }

.has-error .form-control { border-color: rgb(169, 68, 66); box-shadow: rgba=
(0, 0, 0, 0.075) 0px 1px 1px inset; }

.has-error .form-control:focus { border-color: rgb(132, 53, 52); box-shadow=
: rgba(0, 0, 0, 0.075) 0px 1px 1px inset, rgb(206, 132, 131) 0px 0px 6px; }

.has-error .input-group-addon { color: rgb(169, 68, 66); background-color: =
rgb(242, 222, 222); border-color: rgb(169, 68, 66); }

.has-error .form-control-feedback { color: rgb(169, 68, 66); }

.has-feedback label ~ .form-control-feedback { top: 23px; }

.has-feedback label.sr-only ~ .form-control-feedback { top: 0px; }

.help-block { display: block; margin-top: 5px; margin-bottom: 10px; color: =
rgb(64, 64, 64); }

@media (min-width: 768px) {
  .form-inline .form-group { display: inline-block; margin-bottom: 0px; ver=
tical-align: middle; }
  .form-inline .form-control { display: inline-block; width: auto; vertical=
-align: middle; }
  .form-inline .form-control-static { display: inline-block; }
  .form-inline .input-group { display: inline-table; vertical-align: middle=
; }
  .form-inline .input-group .input-group-addon, .form-inline .input-group .=
input-group-btn, .form-inline .input-group .form-control { width: auto; }
  .form-inline .input-group > .form-control { width: 100%; }
  .form-inline .control-label { margin-bottom: 0px; vertical-align: middle;=
 }
  .form-inline .radio, .form-inline .checkbox { display: inline-block; marg=
in-top: 0px; margin-bottom: 0px; vertical-align: middle; }
  .form-inline .radio label, .form-inline .checkbox label { padding-left: 0=
px; }
  .form-inline .radio input[type=3D"radio"], .form-inline .checkbox input[t=
ype=3D"checkbox"] { position: relative; margin-left: 0px; }
  .form-inline .has-feedback .form-control-feedback { top: 0px; }
}

.form-horizontal .radio, .form-horizontal .checkbox, .form-horizontal .radi=
o-inline, .form-horizontal .checkbox-inline { padding-top: 7px; margin-top:=
 0px; margin-bottom: 0px; }

.form-horizontal .radio, .form-horizontal .checkbox { min-height: 25px; }

.form-horizontal .form-group { margin-right: 0px; margin-left: 0px; }

@media (min-width: 768px) {
  .form-horizontal .control-label { padding-top: 7px; margin-bottom: 0px; t=
ext-align: right; }
}

.form-horizontal .has-feedback .form-control-feedback { right: 0px; }

@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label { padding-top: 11px; font-=
size: 17px; }
}

@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label { padding-top: 6px; font-s=
ize: 12px; }
}

.btn { display: inline-block; margin-bottom: 0px; font-weight: normal; text=
-align: center; white-space: nowrap; vertical-align: middle; touch-action: =
manipulation; cursor: pointer; background-image: none; border: 1px solid tr=
ansparent; padding: 6px 12px; font-size: 13px; line-height: 1.42857; border=
-radius: 2px; user-select: none; }

.btn:focus, .btn:active:focus, .btn.active:focus, .btn.focus, .btn:active.f=
ocus, .btn.active.focus { outline: -webkit-focus-ring-color auto 5px; outli=
ne-offset: -2px; }

.btn:hover, .btn:focus, .btn.focus { color: rgb(51, 51, 51); text-decoratio=
n: none; }

.btn:active, .btn.active { background-image: none; outline: 0px; box-shadow=
: rgba(0, 0, 0, 0.125) 0px 3px 5px inset; }

.btn.disabled, .btn[disabled], fieldset[disabled] .btn { cursor: not-allowe=
d; opacity: 0.65; box-shadow: none; }

a.btn.disabled, fieldset[disabled] a.btn { pointer-events: none; }

.btn-default { color: rgb(51, 51, 51); background-color: rgb(255, 255, 255)=
; border-color: rgb(204, 204, 204); }

.btn-default:focus, .btn-default.focus { color: rgb(51, 51, 51); background=
-color: rgb(230, 230, 230); border-color: rgb(140, 140, 140); }

.btn-default:hover { color: rgb(51, 51, 51); background-color: rgb(230, 230=
, 230); border-color: rgb(173, 173, 173); }

.btn-default:active, .btn-default.active, .open > .dropdown-toggle.btn-defa=
ult { color: rgb(51, 51, 51); background-color: rgb(230, 230, 230); backgro=
und-image: none; border-color: rgb(173, 173, 173); }

.btn-default:active:hover, .btn-default.active:hover, .open > .dropdown-tog=
gle.btn-default:hover, .btn-default:active:focus, .btn-default.active:focus=
, .open > .dropdown-toggle.btn-default:focus, .btn-default:active.focus, .b=
tn-default.active.focus, .open > .dropdown-toggle.btn-default.focus { color=
: rgb(51, 51, 51); background-color: rgb(212, 212, 212); border-color: rgb(=
140, 140, 140); }

.btn-default.disabled:hover, .btn-default[disabled]:hover, fieldset[disable=
d] .btn-default:hover, .btn-default.disabled:focus, .btn-default[disabled]:=
focus, fieldset[disabled] .btn-default:focus, .btn-default.disabled.focus, =
.btn-default[disabled].focus, fieldset[disabled] .btn-default.focus { backg=
round-color: rgb(255, 255, 255); border-color: rgb(204, 204, 204); }

.btn-default .badge { color: rgb(255, 255, 255); background-color: rgb(51, =
51, 51); }

.btn-primary { color: rgb(255, 255, 255); background-color: rgb(51, 122, 18=
3); border-color: rgb(46, 109, 164); }

.btn-primary:focus, .btn-primary.focus { color: rgb(255, 255, 255); backgro=
und-color: rgb(40, 96, 144); border-color: rgb(18, 43, 64); }

.btn-primary:hover { color: rgb(255, 255, 255); background-color: rgb(40, 9=
6, 144); border-color: rgb(32, 77, 116); }

.btn-primary:active, .btn-primary.active, .open > .dropdown-toggle.btn-prim=
ary { color: rgb(255, 255, 255); background-color: rgb(40, 96, 144); backgr=
ound-image: none; border-color: rgb(32, 77, 116); }

.btn-primary:active:hover, .btn-primary.active:hover, .open > .dropdown-tog=
gle.btn-primary:hover, .btn-primary:active:focus, .btn-primary.active:focus=
, .open > .dropdown-toggle.btn-primary:focus, .btn-primary:active.focus, .b=
tn-primary.active.focus, .open > .dropdown-toggle.btn-primary.focus { color=
: rgb(255, 255, 255); background-color: rgb(32, 77, 116); border-color: rgb=
(18, 43, 64); }

.btn-primary.disabled:hover, .btn-primary[disabled]:hover, fieldset[disable=
d] .btn-primary:hover, .btn-primary.disabled:focus, .btn-primary[disabled]:=
focus, fieldset[disabled] .btn-primary:focus, .btn-primary.disabled.focus, =
.btn-primary[disabled].focus, fieldset[disabled] .btn-primary.focus { backg=
round-color: rgb(51, 122, 183); border-color: rgb(46, 109, 164); }

.btn-primary .badge { color: rgb(51, 122, 183); background-color: rgb(255, =
255, 255); }

.btn-success { color: rgb(255, 255, 255); background-color: rgb(92, 184, 92=
); border-color: rgb(76, 174, 76); }

.btn-success:focus, .btn-success.focus { color: rgb(255, 255, 255); backgro=
und-color: rgb(68, 157, 68); border-color: rgb(37, 86, 37); }

.btn-success:hover { color: rgb(255, 255, 255); background-color: rgb(68, 1=
57, 68); border-color: rgb(57, 132, 57); }

.btn-success:active, .btn-success.active, .open > .dropdown-toggle.btn-succ=
ess { color: rgb(255, 255, 255); background-color: rgb(68, 157, 68); backgr=
ound-image: none; border-color: rgb(57, 132, 57); }

.btn-success:active:hover, .btn-success.active:hover, .open > .dropdown-tog=
gle.btn-success:hover, .btn-success:active:focus, .btn-success.active:focus=
, .open > .dropdown-toggle.btn-success:focus, .btn-success:active.focus, .b=
tn-success.active.focus, .open > .dropdown-toggle.btn-success.focus { color=
: rgb(255, 255, 255); background-color: rgb(57, 132, 57); border-color: rgb=
(37, 86, 37); }

.btn-success.disabled:hover, .btn-success[disabled]:hover, fieldset[disable=
d] .btn-success:hover, .btn-success.disabled:focus, .btn-success[disabled]:=
focus, fieldset[disabled] .btn-success:focus, .btn-success.disabled.focus, =
.btn-success[disabled].focus, fieldset[disabled] .btn-success.focus { backg=
round-color: rgb(92, 184, 92); border-color: rgb(76, 174, 76); }

.btn-success .badge { color: rgb(92, 184, 92); background-color: rgb(255, 2=
55, 255); }

.btn-info { color: rgb(255, 255, 255); background-color: rgb(91, 192, 222);=
 border-color: rgb(70, 184, 218); }

.btn-info:focus, .btn-info.focus { color: rgb(255, 255, 255); background-co=
lor: rgb(49, 176, 213); border-color: rgb(27, 109, 133); }

.btn-info:hover { color: rgb(255, 255, 255); background-color: rgb(49, 176,=
 213); border-color: rgb(38, 154, 188); }

.btn-info:active, .btn-info.active, .open > .dropdown-toggle.btn-info { col=
or: rgb(255, 255, 255); background-color: rgb(49, 176, 213); background-ima=
ge: none; border-color: rgb(38, 154, 188); }

.btn-info:active:hover, .btn-info.active:hover, .open > .dropdown-toggle.bt=
n-info:hover, .btn-info:active:focus, .btn-info.active:focus, .open > .drop=
down-toggle.btn-info:focus, .btn-info:active.focus, .btn-info.active.focus,=
 .open > .dropdown-toggle.btn-info.focus { color: rgb(255, 255, 255); backg=
round-color: rgb(38, 154, 188); border-color: rgb(27, 109, 133); }

.btn-info.disabled:hover, .btn-info[disabled]:hover, fieldset[disabled] .bt=
n-info:hover, .btn-info.disabled:focus, .btn-info[disabled]:focus, fieldset=
[disabled] .btn-info:focus, .btn-info.disabled.focus, .btn-info[disabled].f=
ocus, fieldset[disabled] .btn-info.focus { background-color: rgb(91, 192, 2=
22); border-color: rgb(70, 184, 218); }

.btn-info .badge { color: rgb(91, 192, 222); background-color: rgb(255, 255=
, 255); }

.btn-warning { color: rgb(255, 255, 255); background-color: rgb(240, 173, 7=
8); border-color: rgb(238, 162, 54); }

.btn-warning:focus, .btn-warning.focus { color: rgb(255, 255, 255); backgro=
und-color: rgb(236, 151, 31); border-color: rgb(152, 95, 13); }

.btn-warning:hover { color: rgb(255, 255, 255); background-color: rgb(236, =
151, 31); border-color: rgb(213, 133, 18); }

.btn-warning:active, .btn-warning.active, .open > .dropdown-toggle.btn-warn=
ing { color: rgb(255, 255, 255); background-color: rgb(236, 151, 31); backg=
round-image: none; border-color: rgb(213, 133, 18); }

.btn-warning:active:hover, .btn-warning.active:hover, .open > .dropdown-tog=
gle.btn-warning:hover, .btn-warning:active:focus, .btn-warning.active:focus=
, .open > .dropdown-toggle.btn-warning:focus, .btn-warning:active.focus, .b=
tn-warning.active.focus, .open > .dropdown-toggle.btn-warning.focus { color=
: rgb(255, 255, 255); background-color: rgb(213, 133, 18); border-color: rg=
b(152, 95, 13); }

.btn-warning.disabled:hover, .btn-warning[disabled]:hover, fieldset[disable=
d] .btn-warning:hover, .btn-warning.disabled:focus, .btn-warning[disabled]:=
focus, fieldset[disabled] .btn-warning:focus, .btn-warning.disabled.focus, =
.btn-warning[disabled].focus, fieldset[disabled] .btn-warning.focus { backg=
round-color: rgb(240, 173, 78); border-color: rgb(238, 162, 54); }

.btn-warning .badge { color: rgb(240, 173, 78); background-color: rgb(255, =
255, 255); }

.btn-danger { color: rgb(255, 255, 255); background-color: rgb(217, 83, 79)=
; border-color: rgb(212, 63, 58); }

.btn-danger:focus, .btn-danger.focus { color: rgb(255, 255, 255); backgroun=
d-color: rgb(201, 48, 44); border-color: rgb(118, 28, 25); }

.btn-danger:hover { color: rgb(255, 255, 255); background-color: rgb(201, 4=
8, 44); border-color: rgb(172, 41, 37); }

.btn-danger:active, .btn-danger.active, .open > .dropdown-toggle.btn-danger=
 { color: rgb(255, 255, 255); background-color: rgb(201, 48, 44); backgroun=
d-image: none; border-color: rgb(172, 41, 37); }

.btn-danger:active:hover, .btn-danger.active:hover, .open > .dropdown-toggl=
e.btn-danger:hover, .btn-danger:active:focus, .btn-danger.active:focus, .op=
en > .dropdown-toggle.btn-danger:focus, .btn-danger:active.focus, .btn-dang=
er.active.focus, .open > .dropdown-toggle.btn-danger.focus { color: rgb(255=
, 255, 255); background-color: rgb(172, 41, 37); border-color: rgb(118, 28,=
 25); }

.btn-danger.disabled:hover, .btn-danger[disabled]:hover, fieldset[disabled]=
 .btn-danger:hover, .btn-danger.disabled:focus, .btn-danger[disabled]:focus=
, fieldset[disabled] .btn-danger:focus, .btn-danger.disabled.focus, .btn-da=
nger[disabled].focus, fieldset[disabled] .btn-danger.focus { background-col=
or: rgb(217, 83, 79); border-color: rgb(212, 63, 58); }

.btn-danger .badge { color: rgb(217, 83, 79); background-color: rgb(255, 25=
5, 255); }

.btn-link { font-weight: 400; color: rgb(41, 110, 170); border-radius: 0px;=
 }

.btn-link, .btn-link:active, .btn-link.active, .btn-link[disabled], fieldse=
t[disabled] .btn-link { background-color: transparent; box-shadow: none; }

.btn-link, .btn-link:hover, .btn-link:focus, .btn-link:active { border-colo=
r: transparent; }

.btn-link:hover, .btn-link:focus { color: rgb(26, 70, 108); text-decoration=
: underline; background-color: transparent; }

.btn-link[disabled]:hover, fieldset[disabled] .btn-link:hover, .btn-link[di=
sabled]:focus, fieldset[disabled] .btn-link:focus { color: rgb(119, 119, 11=
9); text-decoration: none; }

.btn-lg, .btn-group-lg > .btn { padding: 10px 16px; font-size: 17px; line-h=
eight: 1.33333; border-radius: 3px; }

.btn-sm, .btn-group-sm > .btn { padding: 5px 10px; font-size: 12px; line-he=
ight: 1.5; border-radius: 1px; }

.btn-xs, .btn-group-xs > .btn { padding: 1px 5px; font-size: 12px; line-hei=
ght: 1.5; border-radius: 1px; }

.btn-block { display: block; width: 100%; }

.btn-block + .btn-block { margin-top: 5px; }

input[type=3D"submit"].btn-block, input[type=3D"reset"].btn-block, input[ty=
pe=3D"button"].btn-block { width: 100%; }

.fade { opacity: 0; transition: opacity 0.15s linear 0s; }

.fade.in { opacity: 1; }

.collapse { display: none; }

.collapse.in { display: block; }

tr.collapse.in { display: table-row; }

tbody.collapse.in { display: table-row-group; }

.collapsing { position: relative; height: 0px; overflow: hidden; transition=
-property: height, visibility; transition-duration: 0.35s; transition-timin=
g-function: ease; }

.caret { display: inline-block; width: 0px; height: 0px; margin-left: 2px; =
vertical-align: middle; border-top: 4px dashed; border-right: 4px solid tra=
nsparent; border-left: 4px solid transparent; }

.dropup, .dropdown { position: relative; }

.dropdown-toggle:focus { outline: 0px; }

.dropdown-menu { position: absolute; top: 100%; left: 0px; z-index: 1000; d=
isplay: none; float: left; min-width: 160px; padding: 5px 0px; margin: 2px =
0px 0px; font-size: 13px; text-align: left; list-style: none; background-co=
lor: rgb(255, 255, 255); background-clip: padding-box; border: 1px solid rg=
ba(0, 0, 0, 0.15); border-radius: 2px; box-shadow: rgba(0, 0, 0, 0.176) 0px=
 6px 12px; }

.dropdown-menu.pull-right { right: 0px; left: auto; }

.dropdown-menu .divider { height: 1px; margin: 8px 0px; overflow: hidden; b=
ackground-color: rgb(229, 229, 229); }

.dropdown-menu > li > a { display: block; padding: 3px 20px; clear: both; f=
ont-weight: 400; line-height: 1.42857; color: rgb(51, 51, 51); white-space:=
 nowrap; }

.dropdown-menu > li > a:hover, .dropdown-menu > li > a:focus { color: rgb(3=
8, 38, 38); text-decoration: none; background-color: rgb(245, 245, 245); }

.dropdown-menu > .active > a, .dropdown-menu > .active > a:hover, .dropdown=
-menu > .active > a:focus { color: rgb(255, 255, 255); text-decoration: non=
e; background-color: rgb(51, 122, 183); outline: 0px; }

.dropdown-menu > .disabled > a, .dropdown-menu > .disabled > a:hover, .drop=
down-menu > .disabled > a:focus { color: rgb(119, 119, 119); }

.dropdown-menu > .disabled > a:hover, .dropdown-menu > .disabled > a:focus =
{ text-decoration: none; cursor: not-allowed; background-color: transparent=
; background-image: none; }

.open > .dropdown-menu { display: block; }

.open > a { outline: 0px; }

.dropdown-menu-right { right: 0px; left: auto; }

.dropdown-menu-left { right: auto; left: 0px; }

.dropdown-header { display: block; padding: 3px 20px; font-size: 12px; line=
-height: 1.42857; color: rgb(119, 119, 119); white-space: nowrap; }

.dropdown-backdrop { position: fixed; inset: 0px; z-index: 990; }

.pull-right > .dropdown-menu { right: 0px; left: auto; }

.dropup .caret, .navbar-fixed-bottom .dropdown .caret { content: ""; border=
-top: 0px; border-bottom: 4px dashed; }

.dropup .dropdown-menu, .navbar-fixed-bottom .dropdown .dropdown-menu { top=
: auto; bottom: 100%; margin-bottom: 2px; }

@media (min-width: 541px) {
  .navbar-right .dropdown-menu { right: 0px; left: auto; }
  .navbar-right .dropdown-menu-left { right: auto; left: 0px; }
}

.btn-group, .btn-group-vertical { position: relative; display: inline-block=
; vertical-align: middle; }

.btn-group > .btn, .btn-group-vertical > .btn { position: relative; float: =
left; }

.btn-group > .btn:hover, .btn-group-vertical > .btn:hover, .btn-group > .bt=
n:focus, .btn-group-vertical > .btn:focus, .btn-group > .btn:active, .btn-g=
roup-vertical > .btn:active, .btn-group > .btn.active, .btn-group-vertical =
> .btn.active { z-index: 2; }

.btn-group .btn + .btn, .btn-group .btn + .btn-group, .btn-group .btn-group=
 + .btn, .btn-group .btn-group + .btn-group { margin-left: -1px; }

.btn-toolbar { margin-left: -5px; }

.btn-toolbar .btn, .btn-toolbar .btn-group, .btn-toolbar .input-group { flo=
at: left; }

.btn-toolbar > .btn, .btn-toolbar > .btn-group, .btn-toolbar > .input-group=
 { margin-left: 5px; }

.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) =
{ border-radius: 0px; }

.btn-group > .btn:first-child { margin-left: 0px; }

.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) { bord=
er-top-right-radius: 0px; border-bottom-right-radius: 0px; }

.btn-group > .btn:last-child:not(:first-child), .btn-group > .dropdown-togg=
le:not(:first-child) { border-top-left-radius: 0px; border-bottom-left-radi=
us: 0px; }

.btn-group > .btn-group { float: left; }

.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn { border-=
radius: 0px; }

.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child, .bt=
n-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle { bord=
er-top-right-radius: 0px; border-bottom-right-radius: 0px; }

.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child { b=
order-top-left-radius: 0px; border-bottom-left-radius: 0px; }

.btn-group .dropdown-toggle:active, .btn-group.open .dropdown-toggle { outl=
ine: 0px; }

.btn-group > .btn + .dropdown-toggle { padding-right: 8px; padding-left: 8p=
x; }

.btn-group > .btn-lg + .dropdown-toggle { padding-right: 12px; padding-left=
: 12px; }

.btn-group.open .dropdown-toggle { box-shadow: rgba(0, 0, 0, 0.125) 0px 3px=
 5px inset; }

.btn-group.open .dropdown-toggle.btn-link { box-shadow: none; }

.btn .caret { margin-left: 0px; }

.btn-lg .caret { border-width: 5px 5px 0px; }

.dropup .btn-lg .caret { border-width: 0px 5px 5px; }

.btn-group-vertical > .btn, .btn-group-vertical > .btn-group, .btn-group-ve=
rtical > .btn-group > .btn { display: block; float: none; width: 100%; max-=
width: 100%; }

.btn-group-vertical > .btn-group > .btn { float: none; }

.btn-group-vertical > .btn + .btn, .btn-group-vertical > .btn + .btn-group,=
 .btn-group-vertical > .btn-group + .btn, .btn-group-vertical > .btn-group =
+ .btn-group { margin-top: -1px; margin-left: 0px; }

.btn-group-vertical > .btn:not(:first-child):not(:last-child) { border-radi=
us: 0px; }

.btn-group-vertical > .btn:first-child:not(:last-child) { border-radius: 2p=
x 2px 0px 0px; }

.btn-group-vertical > .btn:last-child:not(:first-child) { border-radius: 0p=
x 0px 2px 2px; }

.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn =
{ border-radius: 0px; }

.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-c=
hild, .btn-group-vertical > .btn-group:first-child:not(:last-child) > .drop=
down-toggle { border-bottom-right-radius: 0px; border-bottom-left-radius: 0=
px; }

.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-=
child { border-top-left-radius: 0px; border-top-right-radius: 0px; }

.btn-group-justified { display: table; width: 100%; table-layout: fixed; bo=
rder-collapse: separate; }

.btn-group-justified > .btn, .btn-group-justified > .btn-group { display: t=
able-cell; float: none; width: 1%; }

.btn-group-justified > .btn-group .btn { width: 100%; }

.btn-group-justified > .btn-group .dropdown-menu { left: auto; }

[data-toggle=3D"buttons"] > .btn input[type=3D"radio"], [data-toggle=3D"but=
tons"] > .btn-group > .btn input[type=3D"radio"], [data-toggle=3D"buttons"]=
 > .btn input[type=3D"checkbox"], [data-toggle=3D"buttons"] > .btn-group > =
.btn input[type=3D"checkbox"] { position: absolute; clip: rect(0px, 0px, 0p=
x, 0px); pointer-events: none; }

.input-group { position: relative; display: table; border-collapse: separat=
e; }

.input-group[class*=3D"col-"] { float: none; padding-right: 0px; padding-le=
ft: 0px; }

.input-group .form-control { position: relative; z-index: 2; float: left; w=
idth: 100%; margin-bottom: 0px; }

.input-group .form-control:focus { z-index: 3; }

.input-group-lg > .form-control, .input-group-lg > .input-group-addon, .inp=
ut-group-lg > .input-group-btn > .btn { height: 45px; padding: 10px 16px; f=
ont-size: 17px; line-height: 1.33333; border-radius: 3px; }

select.input-group-lg > .form-control, select.input-group-lg > .input-group=
-addon, select.input-group-lg > .input-group-btn > .btn { height: 45px; lin=
e-height: 45px; }

textarea.input-group-lg > .form-control, textarea.input-group-lg > .input-g=
roup-addon, textarea.input-group-lg > .input-group-btn > .btn, select[multi=
ple].input-group-lg > .form-control, select[multiple].input-group-lg > .inp=
ut-group-addon, select[multiple].input-group-lg > .input-group-btn > .btn {=
 height: auto; }

.input-group-sm > .form-control, .input-group-sm > .input-group-addon, .inp=
ut-group-sm > .input-group-btn > .btn { height: 30px; padding: 5px 10px; fo=
nt-size: 12px; line-height: 1.5; border-radius: 1px; }

select.input-group-sm > .form-control, select.input-group-sm > .input-group=
-addon, select.input-group-sm > .input-group-btn > .btn { height: 30px; lin=
e-height: 30px; }

textarea.input-group-sm > .form-control, textarea.input-group-sm > .input-g=
roup-addon, textarea.input-group-sm > .input-group-btn > .btn, select[multi=
ple].input-group-sm > .form-control, select[multiple].input-group-sm > .inp=
ut-group-addon, select[multiple].input-group-sm > .input-group-btn > .btn {=
 height: auto; }

.input-group-addon, .input-group-btn, .input-group .form-control { display:=
 table-cell; }

.input-group-addon:not(:first-child):not(:last-child), .input-group-btn:not=
(:first-child):not(:last-child), .input-group .form-control:not(:first-chil=
d):not(:last-child) { border-radius: 0px; }

.input-group-addon, .input-group-btn { width: 1%; white-space: nowrap; vert=
ical-align: middle; }

.input-group-addon { padding: 6px 12px; font-size: 13px; font-weight: 400; =
line-height: 1; color: rgb(85, 85, 85); text-align: center; background-colo=
r: rgb(238, 238, 238); border: 1px solid rgb(204, 204, 204); border-radius:=
 2px; }

.input-group-addon.input-sm { padding: 5px 10px; font-size: 12px; border-ra=
dius: 1px; }

.input-group-addon.input-lg { padding: 10px 16px; font-size: 17px; border-r=
adius: 3px; }

.input-group-addon input[type=3D"radio"], .input-group-addon input[type=3D"=
checkbox"] { margin-top: 0px; }

.input-group .form-control:first-child, .input-group-addon:first-child, .in=
put-group-btn:first-child > .btn, .input-group-btn:first-child > .btn-group=
 > .btn, .input-group-btn:first-child > .dropdown-toggle, .input-group-btn:=
last-child > .btn:not(:last-child):not(.dropdown-toggle), .input-group-btn:=
last-child > .btn-group:not(:last-child) > .btn { border-top-right-radius: =
0px; border-bottom-right-radius: 0px; }

.input-group-addon:first-child { border-right: 0px; }

.input-group .form-control:last-child, .input-group-addon:last-child, .inpu=
t-group-btn:last-child > .btn, .input-group-btn:last-child > .btn-group > .=
btn, .input-group-btn:last-child > .dropdown-toggle, .input-group-btn:first=
-child > .btn:not(:first-child), .input-group-btn:first-child > .btn-group:=
not(:first-child) > .btn { border-top-left-radius: 0px; border-bottom-left-=
radius: 0px; }

.input-group-addon:last-child { border-left: 0px; }

.input-group-btn { position: relative; font-size: 0px; white-space: nowrap;=
 }

.input-group-btn > .btn { position: relative; }

.input-group-btn > .btn + .btn { margin-left: -1px; }

.input-group-btn > .btn:hover, .input-group-btn > .btn:focus, .input-group-=
btn > .btn:active { z-index: 2; }

.input-group-btn:first-child > .btn, .input-group-btn:first-child > .btn-gr=
oup { margin-right: -1px; }

.input-group-btn:last-child > .btn, .input-group-btn:last-child > .btn-grou=
p { z-index: 2; margin-left: -1px; }

.nav { padding-left: 0px; margin-bottom: 0px; list-style: none; }

.nav > li { position: relative; display: block; }

.nav > li > a { position: relative; display: block; padding: 10px 15px; }

.nav > li > a:hover, .nav > li > a:focus { text-decoration: none; backgroun=
d-color: rgb(238, 238, 238); }

.nav > li.disabled > a { color: rgb(119, 119, 119); }

.nav > li.disabled > a:hover, .nav > li.disabled > a:focus { color: rgb(119=
, 119, 119); text-decoration: none; cursor: not-allowed; background-color: =
transparent; }

.nav .open > a, .nav .open > a:hover, .nav .open > a:focus { background-col=
or: rgb(238, 238, 238); border-color: rgb(41, 110, 170); }

.nav .nav-divider { height: 1px; margin: 8px 0px; overflow: hidden; backgro=
und-color: rgb(229, 229, 229); }

.nav > li > a > img { max-width: none; }

.nav-tabs { border-bottom: 1px solid rgb(221, 221, 221); }

.nav-tabs > li { float: left; margin-bottom: -1px; }

.nav-tabs > li > a { margin-right: 2px; line-height: 1.42857; border: 1px s=
olid transparent; border-radius: 2px 2px 0px 0px; }

.nav-tabs > li > a:hover { border-color: rgb(238, 238, 238) rgb(238, 238, 2=
38) rgb(221, 221, 221); }

.nav-tabs > li.active > a, .nav-tabs > li.active > a:hover, .nav-tabs > li.=
active > a:focus { color: rgb(85, 85, 85); cursor: default; background-colo=
r: rgb(255, 255, 255); border-width: 1px; border-style: solid; border-color=
: rgb(221, 221, 221) rgb(221, 221, 221) transparent; border-image: initial;=
 }

.nav-tabs.nav-justified { width: 100%; border-bottom: 0px; }

.nav-tabs.nav-justified > li { float: none; }

.nav-tabs.nav-justified > li > a { margin-bottom: 5px; text-align: center; =
}

.nav-tabs.nav-justified > .dropdown .dropdown-menu { top: auto; left: auto;=
 }

@media (min-width: 768px) {
  .nav-tabs.nav-justified > li { display: table-cell; width: 1%; }
  .nav-tabs.nav-justified > li > a { margin-bottom: 0px; }
}

.nav-tabs.nav-justified > li > a { margin-right: 0px; border-radius: 2px; }

.nav-tabs.nav-justified > .active > a, .nav-tabs.nav-justified > .active > =
a:hover, .nav-tabs.nav-justified > .active > a:focus { border: 1px solid rg=
b(221, 221, 221); }

@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a { border-bottom: 1px solid rgb(221, 221,=
 221); border-radius: 2px 2px 0px 0px; }
  .nav-tabs.nav-justified > .active > a, .nav-tabs.nav-justified > .active =
> a:hover, .nav-tabs.nav-justified > .active > a:focus { border-bottom-colo=
r: rgb(255, 255, 255); }
}

.nav-pills > li { float: left; }

.nav-pills > li > a { border-radius: 2px; }

.nav-pills > li + li { margin-left: 2px; }

.nav-pills > li.active > a, .nav-pills > li.active > a:hover, .nav-pills > =
li.active > a:focus { color: rgb(255, 255, 255); background-color: rgb(51, =
122, 183); }

.nav-stacked > li { float: none; }

.nav-stacked > li + li { margin-top: 2px; margin-left: 0px; }

.nav-justified { width: 100%; }

.nav-justified > li { float: none; }

.nav-justified > li > a { margin-bottom: 5px; text-align: center; }

.nav-justified > .dropdown .dropdown-menu { top: auto; left: auto; }

@media (min-width: 768px) {
  .nav-justified > li { display: table-cell; width: 1%; }
  .nav-justified > li > a { margin-bottom: 0px; }
}

.nav-tabs-justified { border-bottom: 0px; }

.nav-tabs-justified > li > a { margin-right: 0px; border-radius: 2px; }

.nav-tabs-justified > .active > a, .nav-tabs-justified > .active > a:hover,=
 .nav-tabs-justified > .active > a:focus { border: 1px solid rgb(221, 221, =
221); }

@media (min-width: 768px) {
  .nav-tabs-justified > li > a { border-bottom: 1px solid rgb(221, 221, 221=
); border-radius: 2px 2px 0px 0px; }
  .nav-tabs-justified > .active > a, .nav-tabs-justified > .active > a:hove=
r, .nav-tabs-justified > .active > a:focus { border-bottom-color: rgb(255, =
255, 255); }
}

.tab-content > .tab-pane { display: none; }

.tab-content > .active { display: block; }

.nav-tabs .dropdown-menu { margin-top: -1px; border-top-left-radius: 0px; b=
order-top-right-radius: 0px; }

.navbar { position: relative; min-height: 30px; margin-bottom: 18px; border=
: 1px solid transparent; }

@media (min-width: 541px) {
  .navbar { border-radius: 2px; }
}

@media (min-width: 541px) {
  .navbar-header { float: left; }
}

.navbar-collapse { padding-right: 0px; padding-left: 0px; overflow-x: visib=
le; border-top: 1px solid transparent; box-shadow: rgba(255, 255, 255, 0.1)=
 0px 1px 0px inset; }

.navbar-collapse.in { overflow-y: auto; }

@media (min-width: 541px) {
  .navbar-collapse { width: auto; border-top: 0px; box-shadow: none; }
  .navbar-collapse.collapse { padding-bottom: 0px; display: block !importan=
t; height: auto !important; overflow: visible !important; }
  .navbar-collapse.in { overflow-y: visible; }
  .navbar-fixed-top .navbar-collapse, .navbar-static-top .navbar-collapse, =
.navbar-fixed-bottom .navbar-collapse { padding-right: 0px; padding-left: 0=
px; }
}

.navbar-fixed-top, .navbar-fixed-bottom { position: fixed; right: 0px; left=
: 0px; z-index: 1030; }

.navbar-fixed-top .navbar-collapse, .navbar-fixed-bottom .navbar-collapse {=
 max-height: 340px; }

@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse, .navbar-fixed-bottom .navbar-collapse=
 { max-height: 200px; }
}

@media (min-width: 541px) {
  .navbar-fixed-top, .navbar-fixed-bottom { border-radius: 0px; }
}

.navbar-fixed-top { top: 0px; border-width: 0px 0px 1px; }

.navbar-fixed-bottom { bottom: 0px; margin-bottom: 0px; border-width: 1px 0=
px 0px; }

.container > .navbar-header, .container-fluid > .navbar-header, .container =
> .navbar-collapse, .container-fluid > .navbar-collapse { margin-right: 0px=
; margin-left: 0px; }

@media (min-width: 541px) {
  .container > .navbar-header, .container-fluid > .navbar-header, .containe=
r > .navbar-collapse, .container-fluid > .navbar-collapse { margin-right: 0=
px; margin-left: 0px; }
}

.navbar-static-top { z-index: 1000; border-width: 0px 0px 1px; }

@media (min-width: 541px) {
  .navbar-static-top { border-radius: 0px; }
}

.navbar-brand { float: left; height: 30px; padding: 6px 0px; font-size: 17p=
x; line-height: 18px; }

.navbar-brand:hover, .navbar-brand:focus { text-decoration: none; }

.navbar-brand > img { display: block; }

@media (min-width: 541px) {
  .navbar > .container .navbar-brand, .navbar > .container-fluid .navbar-br=
and { margin-left: 0px; }
}

.navbar-toggle { position: relative; float: right; padding: 9px 10px; margi=
n-right: 0px; margin-top: -2px; margin-bottom: -2px; background-color: tran=
sparent; background-image: none; border: 1px solid transparent; border-radi=
us: 2px; }

.navbar-toggle:focus { outline: 0px; }

.navbar-toggle .icon-bar { display: block; width: 22px; height: 2px; border=
-radius: 1px; }

.navbar-toggle .icon-bar + .icon-bar { margin-top: 4px; }

@media (min-width: 541px) {
  .navbar-toggle { display: none; }
}

.navbar-nav { margin: 3px 0px; }

.navbar-nav > li > a { padding-top: 10px; padding-bottom: 10px; line-height=
: 18px; }

@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu { position: static; float: none; width: =
auto; margin-top: 0px; background-color: transparent; border: 0px; box-shad=
ow: none; }
  .navbar-nav .open .dropdown-menu > li > a, .navbar-nav .open .dropdown-me=
nu .dropdown-header { padding: 5px 15px 5px 25px; }
  .navbar-nav .open .dropdown-menu > li > a { line-height: 18px; }
  .navbar-nav .open .dropdown-menu > li > a:hover, .navbar-nav .open .dropd=
own-menu > li > a:focus { background-image: none; }
}

@media (min-width: 541px) {
  .navbar-nav { float: left; margin: 0px; }
  .navbar-nav > li { float: left; }
  .navbar-nav > li > a { padding-top: 6px; padding-bottom: 6px; }
}

.navbar-form { padding: 10px 0px; margin: -1px 0px; border-top: 1px solid t=
ransparent; border-bottom: 1px solid transparent; box-shadow: rgba(255, 255=
, 255, 0.1) 0px 1px 0px inset, rgba(255, 255, 255, 0.1) 0px 1px 0px; }

@media (min-width: 768px) {
  .navbar-form .form-group { display: inline-block; margin-bottom: 0px; ver=
tical-align: middle; }
  .navbar-form .form-control { display: inline-block; width: auto; vertical=
-align: middle; }
  .navbar-form .form-control-static { display: inline-block; }
  .navbar-form .input-group { display: inline-table; vertical-align: middle=
; }
  .navbar-form .input-group .input-group-addon, .navbar-form .input-group .=
input-group-btn, .navbar-form .input-group .form-control { width: auto; }
  .navbar-form .input-group > .form-control { width: 100%; }
  .navbar-form .control-label { margin-bottom: 0px; vertical-align: middle;=
 }
  .navbar-form .radio, .navbar-form .checkbox { display: inline-block; marg=
in-top: 0px; margin-bottom: 0px; vertical-align: middle; }
  .navbar-form .radio label, .navbar-form .checkbox label { padding-left: 0=
px; }
  .navbar-form .radio input[type=3D"radio"], .navbar-form .checkbox input[t=
ype=3D"checkbox"] { position: relative; margin-left: 0px; }
  .navbar-form .has-feedback .form-control-feedback { top: 0px; }
}

@media (max-width: 540px) {
  .navbar-form .form-group { margin-bottom: 5px; }
  .navbar-form .form-group:last-child { margin-bottom: 0px; }
}

@media (min-width: 541px) {
  .navbar-form { width: auto; padding-top: 0px; padding-bottom: 0px; margin=
-right: 0px; margin-left: 0px; border: 0px; box-shadow: none; }
}

.navbar-nav > li > .dropdown-menu { margin-top: 0px; border-top-left-radius=
: 0px; border-top-right-radius: 0px; }

.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu { margin-bottom: 0px=
; border-radius: 2px 2px 0px 0px; }

.navbar-btn { margin-top: -1px; margin-bottom: -1px; }

.navbar-btn.btn-sm { margin-top: 0px; margin-bottom: 0px; }

.navbar-btn.btn-xs { margin-top: 4px; margin-bottom: 4px; }

.navbar-text { margin-top: 6px; margin-bottom: 6px; }

@media (min-width: 541px) {
  .navbar-text { float: left; margin-right: 0px; margin-left: 0px; }
}

@media (min-width: 541px) {
  .navbar-left { float: left !important; }
  .navbar-right { margin-right: 0px; float: right !important; }
  .navbar-right ~ .navbar-right { margin-right: 0px; }
}

.navbar-default { background-color: rgb(248, 248, 248); border-color: rgb(2=
31, 231, 231); }

.navbar-default .navbar-brand { color: rgb(86, 86, 86); }

.navbar-default .navbar-brand:hover, .navbar-default .navbar-brand:focus { =
color: rgb(60, 60, 60); background-color: transparent; }

.navbar-default .navbar-text { color: rgb(119, 119, 119); }

.navbar-default .navbar-nav > li > a { color: rgb(86, 86, 86); }

.navbar-default .navbar-nav > li > a:hover, .navbar-default .navbar-nav > l=
i > a:focus { color: rgb(51, 51, 51); background-color: transparent; }

.navbar-default .navbar-nav > .active > a, .navbar-default .navbar-nav > .a=
ctive > a:hover, .navbar-default .navbar-nav > .active > a:focus { color: r=
gb(85, 85, 85); background-color: rgb(231, 231, 231); }

.navbar-default .navbar-nav > .disabled > a, .navbar-default .navbar-nav > =
.disabled > a:hover, .navbar-default .navbar-nav > .disabled > a:focus { co=
lor: rgb(204, 204, 204); background-color: transparent; }

.navbar-default .navbar-nav > .open > a, .navbar-default .navbar-nav > .ope=
n > a:hover, .navbar-default .navbar-nav > .open > a:focus { color: rgb(85,=
 85, 85); background-color: rgb(231, 231, 231); }

@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a { color: rgb(86=
, 86, 86); }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover, .navbar-=
default .navbar-nav .open .dropdown-menu > li > a:focus { color: rgb(51, 51=
, 51); background-color: transparent; }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a, .navbar-d=
efault .navbar-nav .open .dropdown-menu > .active > a:hover, .navbar-defaul=
t .navbar-nav .open .dropdown-menu > .active > a:focus { color: rgb(85, 85,=
 85); background-color: rgb(231, 231, 231); }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a, .navbar=
-default .navbar-nav .open .dropdown-menu > .disabled > a:hover, .navbar-de=
fault .navbar-nav .open .dropdown-menu > .disabled > a:focus { color: rgb(2=
04, 204, 204); background-color: transparent; }
}

.navbar-default .navbar-toggle { border-color: rgb(221, 221, 221); }

.navbar-default .navbar-toggle:hover, .navbar-default .navbar-toggle:focus =
{ background-color: rgb(221, 221, 221); }

.navbar-default .navbar-toggle .icon-bar { background-color: rgb(136, 136, =
136); }

.navbar-default .navbar-collapse, .navbar-default .navbar-form { border-col=
or: rgb(231, 231, 231); }

.navbar-default .navbar-link { color: rgb(86, 86, 86); }

.navbar-default .navbar-link:hover { color: rgb(51, 51, 51); }

.navbar-default .btn-link { color: rgb(86, 86, 86); }

.navbar-default .btn-link:hover, .navbar-default .btn-link:focus { color: r=
gb(51, 51, 51); }

.navbar-default .btn-link[disabled]:hover, fieldset[disabled] .navbar-defau=
lt .btn-link:hover, .navbar-default .btn-link[disabled]:focus, fieldset[dis=
abled] .navbar-default .btn-link:focus { color: rgb(204, 204, 204); }

.navbar-inverse { background-color: rgb(34, 34, 34); border-color: rgb(8, 8=
, 8); }

.navbar-inverse .navbar-brand { color: rgb(157, 157, 157); }

.navbar-inverse .navbar-brand:hover, .navbar-inverse .navbar-brand:focus { =
color: rgb(255, 255, 255); background-color: transparent; }

.navbar-inverse .navbar-text { color: rgb(157, 157, 157); }

.navbar-inverse .navbar-nav > li > a { color: rgb(157, 157, 157); }

.navbar-inverse .navbar-nav > li > a:hover, .navbar-inverse .navbar-nav > l=
i > a:focus { color: rgb(255, 255, 255); background-color: transparent; }

.navbar-inverse .navbar-nav > .active > a, .navbar-inverse .navbar-nav > .a=
ctive > a:hover, .navbar-inverse .navbar-nav > .active > a:focus { color: r=
gb(255, 255, 255); background-color: rgb(8, 8, 8); }

.navbar-inverse .navbar-nav > .disabled > a, .navbar-inverse .navbar-nav > =
.disabled > a:hover, .navbar-inverse .navbar-nav > .disabled > a:focus { co=
lor: rgb(68, 68, 68); background-color: transparent; }

.navbar-inverse .navbar-nav > .open > a, .navbar-inverse .navbar-nav > .ope=
n > a:hover, .navbar-inverse .navbar-nav > .open > a:focus { color: rgb(255=
, 255, 255); background-color: rgb(8, 8, 8); }

@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header { bor=
der-color: rgb(8, 8, 8); }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider { background-co=
lor: rgb(8, 8, 8); }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a { color: rgb(15=
7, 157, 157); }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover, .navbar-=
inverse .navbar-nav .open .dropdown-menu > li > a:focus { color: rgb(255, 2=
55, 255); background-color: transparent; }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a, .navbar-i=
nverse .navbar-nav .open .dropdown-menu > .active > a:hover, .navbar-invers=
e .navbar-nav .open .dropdown-menu > .active > a:focus { color: rgb(255, 25=
5, 255); background-color: rgb(8, 8, 8); }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a, .navbar=
-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover, .navbar-in=
verse .navbar-nav .open .dropdown-menu > .disabled > a:focus { color: rgb(6=
8, 68, 68); background-color: transparent; }
}

.navbar-inverse .navbar-toggle { border-color: rgb(51, 51, 51); }

.navbar-inverse .navbar-toggle:hover, .navbar-inverse .navbar-toggle:focus =
{ background-color: rgb(51, 51, 51); }

.navbar-inverse .navbar-toggle .icon-bar { background-color: rgb(255, 255, =
255); }

.navbar-inverse .navbar-collapse, .navbar-inverse .navbar-form { border-col=
or: rgb(16, 16, 16); }

.navbar-inverse .navbar-link { color: rgb(157, 157, 157); }

.navbar-inverse .navbar-link:hover { color: rgb(255, 255, 255); }

.navbar-inverse .btn-link { color: rgb(157, 157, 157); }

.navbar-inverse .btn-link:hover, .navbar-inverse .btn-link:focus { color: r=
gb(255, 255, 255); }

.navbar-inverse .btn-link[disabled]:hover, fieldset[disabled] .navbar-inver=
se .btn-link:hover, .navbar-inverse .btn-link[disabled]:focus, fieldset[dis=
abled] .navbar-inverse .btn-link:focus { color: rgb(68, 68, 68); }

.breadcrumb { padding: 8px 15px; margin-bottom: 18px; list-style: none; bac=
kground-color: rgb(245, 245, 245); border-radius: 2px; }

.breadcrumb > li { display: inline-block; }

.breadcrumb > li + li::before { padding: 0px 5px; color: rgb(94, 94, 94); c=
ontent: "/=C2=A0"; }

.breadcrumb > .active { color: rgb(119, 119, 119); }

.pagination { display: inline-block; padding-left: 0px; margin: 18px 0px; b=
order-radius: 2px; }

.pagination > li { display: inline; }

.pagination > li > a, .pagination > li > span { position: relative; float: =
left; padding: 6px 12px; margin-left: -1px; line-height: 1.42857; color: rg=
b(41, 110, 170); text-decoration: none; background-color: rgb(255, 255, 255=
); border: 1px solid rgb(221, 221, 221); }

.pagination > li > a:hover, .pagination > li > span:hover, .pagination > li=
 > a:focus, .pagination > li > span:focus { z-index: 2; color: rgb(26, 70, =
108); background-color: rgb(238, 238, 238); border-color: rgb(221, 221, 221=
); }

.pagination > li:first-child > a, .pagination > li:first-child > span { mar=
gin-left: 0px; border-top-left-radius: 2px; border-bottom-left-radius: 2px;=
 }

.pagination > li:last-child > a, .pagination > li:last-child > span { borde=
r-top-right-radius: 2px; border-bottom-right-radius: 2px; }

.pagination > .active > a, .pagination > .active > span, .pagination > .act=
ive > a:hover, .pagination > .active > span:hover, .pagination > .active > =
a:focus, .pagination > .active > span:focus { z-index: 3; color: rgb(255, 2=
55, 255); cursor: default; background-color: rgb(51, 122, 183); border-colo=
r: rgb(51, 122, 183); }

.pagination > .disabled > span, .pagination > .disabled > span:hover, .pagi=
nation > .disabled > span:focus, .pagination > .disabled > a, .pagination >=
 .disabled > a:hover, .pagination > .disabled > a:focus { color: rgb(119, 1=
19, 119); cursor: not-allowed; background-color: rgb(255, 255, 255); border=
-color: rgb(221, 221, 221); }

.pagination-lg > li > a, .pagination-lg > li > span { padding: 10px 16px; f=
ont-size: 17px; line-height: 1.33333; }

.pagination-lg > li:first-child > a, .pagination-lg > li:first-child > span=
 { border-top-left-radius: 3px; border-bottom-left-radius: 3px; }

.pagination-lg > li:last-child > a, .pagination-lg > li:last-child > span {=
 border-top-right-radius: 3px; border-bottom-right-radius: 3px; }

.pagination-sm > li > a, .pagination-sm > li > span { padding: 5px 10px; fo=
nt-size: 12px; line-height: 1.5; }

.pagination-sm > li:first-child > a, .pagination-sm > li:first-child > span=
 { border-top-left-radius: 1px; border-bottom-left-radius: 1px; }

.pagination-sm > li:last-child > a, .pagination-sm > li:last-child > span {=
 border-top-right-radius: 1px; border-bottom-right-radius: 1px; }

.pager { padding-left: 0px; margin: 18px 0px; text-align: center; list-styl=
e: none; }

.pager li { display: inline; }

.pager li > a, .pager li > span { display: inline-block; padding: 5px 14px;=
 background-color: rgb(255, 255, 255); border: 1px solid rgb(221, 221, 221)=
; border-radius: 15px; }

.pager li > a:hover, .pager li > a:focus { text-decoration: none; backgroun=
d-color: rgb(238, 238, 238); }

.pager .next > a, .pager .next > span { float: right; }

.pager .previous > a, .pager .previous > span { float: left; }

.pager .disabled > a, .pager .disabled > a:hover, .pager .disabled > a:focu=
s, .pager .disabled > span { color: rgb(119, 119, 119); cursor: not-allowed=
; background-color: rgb(255, 255, 255); }

.label { display: inline; padding: 0.2em 0.6em 0.3em; font-size: 75%; font-=
weight: 700; line-height: 1; color: rgb(255, 255, 255); text-align: center;=
 white-space: nowrap; vertical-align: baseline; border-radius: 0.25em; }

a.label:hover, a.label:focus { color: rgb(255, 255, 255); text-decoration: =
none; cursor: pointer; }

.label:empty { display: none; }

.btn .label { position: relative; top: -1px; }

.label-default { background-color: rgb(119, 119, 119); }

.label-default[href]:hover, .label-default[href]:focus { background-color: =
rgb(94, 94, 94); }

.label-primary { background-color: rgb(51, 122, 183); }

.label-primary[href]:hover, .label-primary[href]:focus { background-color: =
rgb(40, 96, 144); }

.label-success { background-color: rgb(92, 184, 92); }

.label-success[href]:hover, .label-success[href]:focus { background-color: =
rgb(68, 157, 68); }

.label-info { background-color: rgb(91, 192, 222); }

.label-info[href]:hover, .label-info[href]:focus { background-color: rgb(49=
, 176, 213); }

.label-warning { background-color: rgb(240, 173, 78); }

.label-warning[href]:hover, .label-warning[href]:focus { background-color: =
rgb(236, 151, 31); }

.label-danger { background-color: rgb(217, 83, 79); }

.label-danger[href]:hover, .label-danger[href]:focus { background-color: rg=
b(201, 48, 44); }

.badge { display: inline-block; min-width: 10px; padding: 3px 7px; font-siz=
e: 12px; font-weight: bold; line-height: 1; color: rgb(255, 255, 255); text=
-align: center; white-space: nowrap; vertical-align: middle; background-col=
or: rgb(119, 119, 119); border-radius: 10px; }

.badge:empty { display: none; }

.btn .badge { position: relative; top: -1px; }

.btn-xs .badge, .btn-group-xs > .btn .badge { top: 0px; padding: 1px 5px; }

a.badge:hover, a.badge:focus { color: rgb(255, 255, 255); text-decoration: =
none; cursor: pointer; }

.list-group-item.active > .badge, .nav-pills > .active > a > .badge { color=
: rgb(41, 110, 170); background-color: rgb(255, 255, 255); }

.list-group-item > .badge { float: right; }

.list-group-item > .badge + .badge { margin-right: 5px; }

.nav-pills > li > a > .badge { margin-left: 3px; }

.jumbotron { padding-top: 30px; padding-bottom: 30px; margin-bottom: 30px; =
color: inherit; background-color: rgb(238, 238, 238); }

.jumbotron h1, .jumbotron .h1 { color: inherit; }

.jumbotron p { margin-bottom: 15px; font-size: 20px; font-weight: 200; }

.jumbotron > hr { border-top-color: rgb(213, 213, 213); }

.container .jumbotron, .container-fluid .jumbotron { padding-right: 0px; pa=
dding-left: 0px; border-radius: 3px; }

.jumbotron .container { max-width: 100%; }

@media screen and (min-width: 768px) {
  .jumbotron { padding-top: 48px; padding-bottom: 48px; }
  .container .jumbotron, .container-fluid .jumbotron { padding-right: 60px;=
 padding-left: 60px; }
  .jumbotron h1, .jumbotron .h1 { font-size: 59px; }
}

.thumbnail { display: block; padding: 4px; margin-bottom: 18px; line-height=
: 1.42857; background-color: rgb(255, 255, 255); border: 1px solid rgb(221,=
 221, 221); border-radius: 2px; transition: border 0.2s ease-in-out 0s; }

.thumbnail > img, .thumbnail a > img { margin-right: auto; margin-left: aut=
o; }

a.thumbnail:hover, a.thumbnail:focus, a.thumbnail.active { border-color: rg=
b(41, 110, 170); }

.thumbnail .caption { padding: 9px; color: rgb(0, 0, 0); }

.alert { padding: 15px; margin-bottom: 18px; border: 1px solid transparent;=
 border-radius: 2px; }

.alert h4 { margin-top: 0px; color: inherit; }

.alert .alert-link { font-weight: bold; }

.alert > p, .alert > ul { margin-bottom: 0px; }

.alert > p + p { margin-top: 5px; }

.alert-dismissable, .alert-dismissible { padding-right: 35px; }

.alert-dismissable .close, .alert-dismissible .close { position: relative; =
top: -2px; right: -21px; color: inherit; }

.alert-success { color: rgb(60, 118, 61); background-color: rgb(223, 240, 2=
16); border-color: rgb(214, 233, 198); }

.alert-success hr { border-top-color: rgb(201, 226, 179); }

.alert-success .alert-link { color: rgb(43, 84, 44); }

.alert-info { color: rgb(49, 112, 143); background-color: rgb(217, 237, 247=
); border-color: rgb(188, 232, 241); }

.alert-info hr { border-top-color: rgb(166, 225, 236); }

.alert-info .alert-link { color: rgb(36, 82, 105); }

.alert-warning { color: rgb(138, 109, 59); background-color: rgb(252, 248, =
227); border-color: rgb(250, 235, 204); }

.alert-warning hr { border-top-color: rgb(247, 225, 181); }

.alert-warning .alert-link { color: rgb(102, 81, 44); }

.alert-danger { color: rgb(169, 68, 66); background-color: rgb(242, 222, 22=
2); border-color: rgb(235, 204, 209); }

.alert-danger hr { border-top-color: rgb(228, 185, 192); }

.alert-danger .alert-link { color: rgb(132, 53, 52); }

@-webkit-keyframes progress-bar-stripes {=20
  0% { background-position: 40px 0px; }
  100% { background-position: 0px 0px; }
}

@keyframes progress-bar-stripes {=20
  0% { background-position: 40px 0px; }
  100% { background-position: 0px 0px; }
}

.progress { height: 18px; margin-bottom: 18px; overflow: hidden; background=
-color: rgb(245, 245, 245); border-radius: 2px; box-shadow: rgba(0, 0, 0, 0=
.1) 0px 1px 2px inset; }

.progress-bar { float: left; width: 0%; height: 100%; font-size: 12px; line=
-height: 18px; color: rgb(255, 255, 255); text-align: center; background-co=
lor: rgb(51, 122, 183); box-shadow: rgba(0, 0, 0, 0.15) 0px -1px 0px inset;=
 transition: width 0.6s ease 0s; }

.progress-striped .progress-bar, .progress-bar-striped { background-image: =
linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, tran=
sparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, =
transparent 75%, transparent); background-size: 40px 40px; }

.progress.active .progress-bar, .progress-bar.active { animation: 2s linear=
 0s infinite normal none running progress-bar-stripes; }

.progress-bar-success { background-color: rgb(92, 184, 92); }

.progress-striped .progress-bar-success { background-image: linear-gradient=
(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rg=
ba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%=
, transparent); }

.progress-bar-info { background-color: rgb(91, 192, 222); }

.progress-striped .progress-bar-info { background-image: linear-gradient(45=
deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(=
255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, t=
ransparent); }

.progress-bar-warning { background-color: rgb(240, 173, 78); }

.progress-striped .progress-bar-warning { background-image: linear-gradient=
(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rg=
ba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%=
, transparent); }

.progress-bar-danger { background-color: rgb(217, 83, 79); }

.progress-striped .progress-bar-danger { background-image: linear-gradient(=
45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgb=
a(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%,=
 transparent); }

.media { margin-top: 15px; }

.media:first-child { margin-top: 0px; }

.media, .media-body { overflow: hidden; zoom: 1; }

.media-body { width: 10000px; }

.media-object { display: block; }

.media-object.img-thumbnail { max-width: none; }

.media-right, .media > .pull-right { padding-left: 10px; }

.media-left, .media > .pull-left { padding-right: 10px; }

.media-left, .media-right, .media-body { display: table-cell; vertical-alig=
n: top; }

.media-middle { vertical-align: middle; }

.media-bottom { vertical-align: bottom; }

.media-heading { margin-top: 0px; margin-bottom: 5px; }

.media-list { padding-left: 0px; list-style: none; }

.list-group { padding-left: 0px; margin-bottom: 20px; }

.list-group-item { position: relative; display: block; padding: 10px 15px; =
margin-bottom: -1px; background-color: rgb(255, 255, 255); border: 1px soli=
d rgb(221, 221, 221); }

.list-group-item:first-child { border-top-left-radius: 2px; border-top-righ=
t-radius: 2px; }

.list-group-item:last-child { margin-bottom: 0px; border-bottom-right-radiu=
s: 2px; border-bottom-left-radius: 2px; }

.list-group-item.disabled, .list-group-item.disabled:hover, .list-group-ite=
m.disabled:focus { color: rgb(119, 119, 119); cursor: not-allowed; backgrou=
nd-color: rgb(238, 238, 238); }

.list-group-item.disabled .list-group-item-heading, .list-group-item.disabl=
ed:hover .list-group-item-heading, .list-group-item.disabled:focus .list-gr=
oup-item-heading { color: inherit; }

.list-group-item.disabled .list-group-item-text, .list-group-item.disabled:=
hover .list-group-item-text, .list-group-item.disabled:focus .list-group-it=
em-text { color: rgb(119, 119, 119); }

.list-group-item.active, .list-group-item.active:hover, .list-group-item.ac=
tive:focus { z-index: 2; color: rgb(255, 255, 255); background-color: rgb(5=
1, 122, 183); border-color: rgb(51, 122, 183); }

.list-group-item.active .list-group-item-heading, .list-group-item.active:h=
over .list-group-item-heading, .list-group-item.active:focus .list-group-it=
em-heading, .list-group-item.active .list-group-item-heading > small, .list=
-group-item.active:hover .list-group-item-heading > small, .list-group-item=
.active:focus .list-group-item-heading > small, .list-group-item.active .li=
st-group-item-heading > .small, .list-group-item.active:hover .list-group-i=
tem-heading > .small, .list-group-item.active:focus .list-group-item-headin=
g > .small { color: inherit; }

.list-group-item.active .list-group-item-text, .list-group-item.active:hove=
r .list-group-item-text, .list-group-item.active:focus .list-group-item-tex=
t { color: rgb(199, 221, 239); }

a.list-group-item, button.list-group-item { color: rgb(85, 85, 85); }

a.list-group-item .list-group-item-heading, button.list-group-item .list-gr=
oup-item-heading { color: rgb(51, 51, 51); }

a.list-group-item:hover, button.list-group-item:hover, a.list-group-item:fo=
cus, button.list-group-item:focus { color: rgb(85, 85, 85); text-decoration=
: none; background-color: rgb(245, 245, 245); }

button.list-group-item { width: 100%; text-align: left; }

.list-group-item-success { color: rgb(60, 118, 61); background-color: rgb(2=
23, 240, 216); }

a.list-group-item-success, button.list-group-item-success { color: rgb(60, =
118, 61); }

a.list-group-item-success .list-group-item-heading, button.list-group-item-=
success .list-group-item-heading { color: inherit; }

a.list-group-item-success:hover, button.list-group-item-success:hover, a.li=
st-group-item-success:focus, button.list-group-item-success:focus { color: =
rgb(60, 118, 61); background-color: rgb(208, 233, 198); }

a.list-group-item-success.active, button.list-group-item-success.active, a.=
list-group-item-success.active:hover, button.list-group-item-success.active=
:hover, a.list-group-item-success.active:focus, button.list-group-item-succ=
ess.active:focus { color: rgb(255, 255, 255); background-color: rgb(60, 118=
, 61); border-color: rgb(60, 118, 61); }

.list-group-item-info { color: rgb(49, 112, 143); background-color: rgb(217=
, 237, 247); }

a.list-group-item-info, button.list-group-item-info { color: rgb(49, 112, 1=
43); }

a.list-group-item-info .list-group-item-heading, button.list-group-item-inf=
o .list-group-item-heading { color: inherit; }

a.list-group-item-info:hover, button.list-group-item-info:hover, a.list-gro=
up-item-info:focus, button.list-group-item-info:focus { color: rgb(49, 112,=
 143); background-color: rgb(196, 227, 243); }

a.list-group-item-info.active, button.list-group-item-info.active, a.list-g=
roup-item-info.active:hover, button.list-group-item-info.active:hover, a.li=
st-group-item-info.active:focus, button.list-group-item-info.active:focus {=
 color: rgb(255, 255, 255); background-color: rgb(49, 112, 143); border-col=
or: rgb(49, 112, 143); }

.list-group-item-warning { color: rgb(138, 109, 59); background-color: rgb(=
252, 248, 227); }

a.list-group-item-warning, button.list-group-item-warning { color: rgb(138,=
 109, 59); }

a.list-group-item-warning .list-group-item-heading, button.list-group-item-=
warning .list-group-item-heading { color: inherit; }

a.list-group-item-warning:hover, button.list-group-item-warning:hover, a.li=
st-group-item-warning:focus, button.list-group-item-warning:focus { color: =
rgb(138, 109, 59); background-color: rgb(250, 242, 204); }

a.list-group-item-warning.active, button.list-group-item-warning.active, a.=
list-group-item-warning.active:hover, button.list-group-item-warning.active=
:hover, a.list-group-item-warning.active:focus, button.list-group-item-warn=
ing.active:focus { color: rgb(255, 255, 255); background-color: rgb(138, 10=
9, 59); border-color: rgb(138, 109, 59); }

.list-group-item-danger { color: rgb(169, 68, 66); background-color: rgb(24=
2, 222, 222); }

a.list-group-item-danger, button.list-group-item-danger { color: rgb(169, 6=
8, 66); }

a.list-group-item-danger .list-group-item-heading, button.list-group-item-d=
anger .list-group-item-heading { color: inherit; }

a.list-group-item-danger:hover, button.list-group-item-danger:hover, a.list=
-group-item-danger:focus, button.list-group-item-danger:focus { color: rgb(=
169, 68, 66); background-color: rgb(235, 204, 204); }

a.list-group-item-danger.active, button.list-group-item-danger.active, a.li=
st-group-item-danger.active:hover, button.list-group-item-danger.active:hov=
er, a.list-group-item-danger.active:focus, button.list-group-item-danger.ac=
tive:focus { color: rgb(255, 255, 255); background-color: rgb(169, 68, 66);=
 border-color: rgb(169, 68, 66); }

.list-group-item-heading { margin-top: 0px; margin-bottom: 5px; }

.list-group-item-text { margin-bottom: 0px; line-height: 1.3; }

.panel { margin-bottom: 18px; background-color: rgb(255, 255, 255); border:=
 1px solid transparent; border-radius: 2px; box-shadow: rgba(0, 0, 0, 0.05)=
 0px 1px 1px; }

.panel-body { padding: 15px; }

.panel-heading { padding: 10px 15px; border-bottom: 1px solid transparent; =
border-top-left-radius: 1px; border-top-right-radius: 1px; }

.panel-heading > .dropdown .dropdown-toggle { color: inherit; }

.panel-title { margin-top: 0px; margin-bottom: 0px; font-size: 15px; color:=
 inherit; }

.panel-title > a, .panel-title > small, .panel-title > .small, .panel-title=
 > small > a, .panel-title > .small > a { color: inherit; }

.panel-footer { padding: 10px 15px; background-color: rgb(245, 245, 245); b=
order-top: 1px solid rgb(221, 221, 221); border-bottom-right-radius: 1px; b=
order-bottom-left-radius: 1px; }

.panel > .list-group, .panel > .panel-collapse > .list-group { margin-botto=
m: 0px; }

.panel > .list-group .list-group-item, .panel > .panel-collapse > .list-gro=
up .list-group-item { border-width: 1px 0px; border-radius: 0px; }

.panel > .list-group:first-child .list-group-item:first-child, .panel > .pa=
nel-collapse > .list-group:first-child .list-group-item:first-child { borde=
r-top: 0px; border-top-left-radius: 1px; border-top-right-radius: 1px; }

.panel > .list-group:last-child .list-group-item:last-child, .panel > .pane=
l-collapse > .list-group:last-child .list-group-item:last-child { border-bo=
ttom: 0px; border-bottom-right-radius: 1px; border-bottom-left-radius: 1px;=
 }

.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:fi=
rst-child { border-top-left-radius: 0px; border-top-right-radius: 0px; }

.panel-heading + .list-group .list-group-item:first-child { border-top-widt=
h: 0px; }

.list-group + .panel-footer { border-top-width: 0px; }

.panel > .table, .panel > .table-responsive > .table, .panel > .panel-colla=
pse > .table { margin-bottom: 0px; }

.panel > .table caption, .panel > .table-responsive > .table caption, .pane=
l > .panel-collapse > .table caption { padding-right: 15px; padding-left: 1=
5px; }

.panel > .table:first-child, .panel > .table-responsive:first-child > .tabl=
e:first-child { border-top-left-radius: 1px; border-top-right-radius: 1px; =
}

.panel > .table:first-child > thead:first-child > tr:first-child, .panel > =
.table-responsive:first-child > .table:first-child > thead:first-child > tr=
:first-child, .panel > .table:first-child > tbody:first-child > tr:first-ch=
ild, .panel > .table-responsive:first-child > .table:first-child > tbody:fi=
rst-child > tr:first-child { border-top-left-radius: 1px; border-top-right-=
radius: 1px; }

.panel > .table:first-child > thead:first-child > tr:first-child td:first-c=
hild, .panel > .table-responsive:first-child > .table:first-child > thead:f=
irst-child > tr:first-child td:first-child, .panel > .table:first-child > t=
body:first-child > tr:first-child td:first-child, .panel > .table-responsiv=
e:first-child > .table:first-child > tbody:first-child > tr:first-child td:=
first-child, .panel > .table:first-child > thead:first-child > tr:first-chi=
ld th:first-child, .panel > .table-responsive:first-child > .table:first-ch=
ild > thead:first-child > tr:first-child th:first-child, .panel > .table:fi=
rst-child > tbody:first-child > tr:first-child th:first-child, .panel > .ta=
ble-responsive:first-child > .table:first-child > tbody:first-child > tr:fi=
rst-child th:first-child { border-top-left-radius: 1px; }

.panel > .table:first-child > thead:first-child > tr:first-child td:last-ch=
ild, .panel > .table-responsive:first-child > .table:first-child > thead:fi=
rst-child > tr:first-child td:last-child, .panel > .table:first-child > tbo=
dy:first-child > tr:first-child td:last-child, .panel > .table-responsive:f=
irst-child > .table:first-child > tbody:first-child > tr:first-child td:las=
t-child, .panel > .table:first-child > thead:first-child > tr:first-child t=
h:last-child, .panel > .table-responsive:first-child > .table:first-child >=
 thead:first-child > tr:first-child th:last-child, .panel > .table:first-ch=
ild > tbody:first-child > tr:first-child th:last-child, .panel > .table-res=
ponsive:first-child > .table:first-child > tbody:first-child > tr:first-chi=
ld th:last-child { border-top-right-radius: 1px; }

.panel > .table:last-child, .panel > .table-responsive:last-child > .table:=
last-child { border-bottom-right-radius: 1px; border-bottom-left-radius: 1p=
x; }

.panel > .table:last-child > tbody:last-child > tr:last-child, .panel > .ta=
ble-responsive:last-child > .table:last-child > tbody:last-child > tr:last-=
child, .panel > .table:last-child > tfoot:last-child > tr:last-child, .pane=
l > .table-responsive:last-child > .table:last-child > tfoot:last-child > t=
r:last-child { border-bottom-right-radius: 1px; border-bottom-left-radius: =
1px; }

.panel > .table:last-child > tbody:last-child > tr:last-child td:first-chil=
d, .panel > .table-responsive:last-child > .table:last-child > tbody:last-c=
hild > tr:last-child td:first-child, .panel > .table:last-child > tfoot:las=
t-child > tr:last-child td:first-child, .panel > .table-responsive:last-chi=
ld > .table:last-child > tfoot:last-child > tr:last-child td:first-child, .=
panel > .table:last-child > tbody:last-child > tr:last-child th:first-child=
, .panel > .table-responsive:last-child > .table:last-child > tbody:last-ch=
ild > tr:last-child th:first-child, .panel > .table:last-child > tfoot:last=
-child > tr:last-child th:first-child, .panel > .table-responsive:last-chil=
d > .table:last-child > tfoot:last-child > tr:last-child th:first-child { b=
order-bottom-left-radius: 1px; }

.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child=
, .panel > .table-responsive:last-child > .table:last-child > tbody:last-ch=
ild > tr:last-child td:last-child, .panel > .table:last-child > tfoot:last-=
child > tr:last-child td:last-child, .panel > .table-responsive:last-child =
> .table:last-child > tfoot:last-child > tr:last-child td:last-child, .pane=
l > .table:last-child > tbody:last-child > tr:last-child th:last-child, .pa=
nel > .table-responsive:last-child > .table:last-child > tbody:last-child >=
 tr:last-child th:last-child, .panel > .table:last-child > tfoot:last-child=
 > tr:last-child th:last-child, .panel > .table-responsive:last-child > .ta=
ble:last-child > tfoot:last-child > tr:last-child th:last-child { border-bo=
ttom-right-radius: 1px; }

.panel > .panel-body + .table, .panel > .panel-body + .table-responsive, .p=
anel > .table + .panel-body, .panel > .table-responsive + .panel-body { bor=
der-top: 1px solid rgb(221, 221, 221); }

.panel > .table > tbody:first-child > tr:first-child th, .panel > .table > =
tbody:first-child > tr:first-child td { border-top: 0px; }

.panel > .table-bordered, .panel > .table-responsive > .table-bordered { bo=
rder: 0px; }

.panel > .table-bordered > thead > tr > th:first-child, .panel > .table-res=
ponsive > .table-bordered > thead > tr > th:first-child, .panel > .table-bo=
rdered > tbody > tr > th:first-child, .panel > .table-responsive > .table-b=
ordered > tbody > tr > th:first-child, .panel > .table-bordered > tfoot > t=
r > th:first-child, .panel > .table-responsive > .table-bordered > tfoot > =
tr > th:first-child, .panel > .table-bordered > thead > tr > td:first-child=
, .panel > .table-responsive > .table-bordered > thead > tr > td:first-chil=
d, .panel > .table-bordered > tbody > tr > td:first-child, .panel > .table-=
responsive > .table-bordered > tbody > tr > td:first-child, .panel > .table=
-bordered > tfoot > tr > td:first-child, .panel > .table-responsive > .tabl=
e-bordered > tfoot > tr > td:first-child { border-left: 0px; }

.panel > .table-bordered > thead > tr > th:last-child, .panel > .table-resp=
onsive > .table-bordered > thead > tr > th:last-child, .panel > .table-bord=
ered > tbody > tr > th:last-child, .panel > .table-responsive > .table-bord=
ered > tbody > tr > th:last-child, .panel > .table-bordered > tfoot > tr > =
th:last-child, .panel > .table-responsive > .table-bordered > tfoot > tr > =
th:last-child, .panel > .table-bordered > thead > tr > td:last-child, .pane=
l > .table-responsive > .table-bordered > thead > tr > td:last-child, .pane=
l > .table-bordered > tbody > tr > td:last-child, .panel > .table-responsiv=
e > .table-bordered > tbody > tr > td:last-child, .panel > .table-bordered =
> tfoot > tr > td:last-child, .panel > .table-responsive > .table-bordered =
> tfoot > tr > td:last-child { border-right: 0px; }

.panel > .table-bordered > thead > tr:first-child > td, .panel > .table-res=
ponsive > .table-bordered > thead > tr:first-child > td, .panel > .table-bo=
rdered > tbody > tr:first-child > td, .panel > .table-responsive > .table-b=
ordered > tbody > tr:first-child > td, .panel > .table-bordered > thead > t=
r:first-child > th, .panel > .table-responsive > .table-bordered > thead > =
tr:first-child > th, .panel > .table-bordered > tbody > tr:first-child > th=
, .panel > .table-responsive > .table-bordered > tbody > tr:first-child > t=
h { border-bottom: 0px; }

.panel > .table-bordered > tbody > tr:last-child > td, .panel > .table-resp=
onsive > .table-bordered > tbody > tr:last-child > td, .panel > .table-bord=
ered > tfoot > tr:last-child > td, .panel > .table-responsive > .table-bord=
ered > tfoot > tr:last-child > td, .panel > .table-bordered > tbody > tr:la=
st-child > th, .panel > .table-responsive > .table-bordered > tbody > tr:la=
st-child > th, .panel > .table-bordered > tfoot > tr:last-child > th, .pane=
l > .table-responsive > .table-bordered > tfoot > tr:last-child > th { bord=
er-bottom: 0px; }

.panel > .table-responsive { margin-bottom: 0px; border: 0px; }

.panel-group { margin-bottom: 18px; }

.panel-group .panel { margin-bottom: 0px; border-radius: 2px; }

.panel-group .panel + .panel { margin-top: 5px; }

.panel-group .panel-heading { border-bottom: 0px; }

.panel-group .panel-heading + .panel-collapse > .panel-body, .panel-group .=
panel-heading + .panel-collapse > .list-group { border-top: 1px solid rgb(2=
21, 221, 221); }

.panel-group .panel-footer { border-top: 0px; }

.panel-group .panel-footer + .panel-collapse .panel-body { border-bottom: 1=
px solid rgb(221, 221, 221); }

.panel-default { border-color: rgb(221, 221, 221); }

.panel-default > .panel-heading { color: rgb(51, 51, 51); background-color:=
 rgb(245, 245, 245); border-color: rgb(221, 221, 221); }

.panel-default > .panel-heading + .panel-collapse > .panel-body { border-to=
p-color: rgb(221, 221, 221); }

.panel-default > .panel-heading .badge { color: rgb(245, 245, 245); backgro=
und-color: rgb(51, 51, 51); }

.panel-default > .panel-footer + .panel-collapse > .panel-body { border-bot=
tom-color: rgb(221, 221, 221); }

.panel-primary { border-color: rgb(51, 122, 183); }

.panel-primary > .panel-heading { color: rgb(255, 255, 255); background-col=
or: rgb(51, 122, 183); border-color: rgb(51, 122, 183); }

.panel-primary > .panel-heading + .panel-collapse > .panel-body { border-to=
p-color: rgb(51, 122, 183); }

.panel-primary > .panel-heading .badge { color: rgb(51, 122, 183); backgrou=
nd-color: rgb(255, 255, 255); }

.panel-primary > .panel-footer + .panel-collapse > .panel-body { border-bot=
tom-color: rgb(51, 122, 183); }

.panel-success { border-color: rgb(214, 233, 198); }

.panel-success > .panel-heading { color: rgb(60, 118, 61); background-color=
: rgb(223, 240, 216); border-color: rgb(214, 233, 198); }

.panel-success > .panel-heading + .panel-collapse > .panel-body { border-to=
p-color: rgb(214, 233, 198); }

.panel-success > .panel-heading .badge { color: rgb(223, 240, 216); backgro=
und-color: rgb(60, 118, 61); }

.panel-success > .panel-footer + .panel-collapse > .panel-body { border-bot=
tom-color: rgb(214, 233, 198); }

.panel-info { border-color: rgb(188, 232, 241); }

.panel-info > .panel-heading { color: rgb(49, 112, 143); background-color: =
rgb(217, 237, 247); border-color: rgb(188, 232, 241); }

.panel-info > .panel-heading + .panel-collapse > .panel-body { border-top-c=
olor: rgb(188, 232, 241); }

.panel-info > .panel-heading .badge { color: rgb(217, 237, 247); background=
-color: rgb(49, 112, 143); }

.panel-info > .panel-footer + .panel-collapse > .panel-body { border-bottom=
-color: rgb(188, 232, 241); }

.panel-warning { border-color: rgb(250, 235, 204); }

.panel-warning > .panel-heading { color: rgb(138, 109, 59); background-colo=
r: rgb(252, 248, 227); border-color: rgb(250, 235, 204); }

.panel-warning > .panel-heading + .panel-collapse > .panel-body { border-to=
p-color: rgb(250, 235, 204); }

.panel-warning > .panel-heading .badge { color: rgb(252, 248, 227); backgro=
und-color: rgb(138, 109, 59); }

.panel-warning > .panel-footer + .panel-collapse > .panel-body { border-bot=
tom-color: rgb(250, 235, 204); }

.panel-danger { border-color: rgb(235, 204, 209); }

.panel-danger > .panel-heading { color: rgb(169, 68, 66); background-color:=
 rgb(242, 222, 222); border-color: rgb(235, 204, 209); }

.panel-danger > .panel-heading + .panel-collapse > .panel-body { border-top=
-color: rgb(235, 204, 209); }

.panel-danger > .panel-heading .badge { color: rgb(242, 222, 222); backgrou=
nd-color: rgb(169, 68, 66); }

.panel-danger > .panel-footer + .panel-collapse > .panel-body { border-bott=
om-color: rgb(235, 204, 209); }

.embed-responsive { position: relative; display: block; height: 0px; paddin=
g: 0px; overflow: hidden; }

.embed-responsive .embed-responsive-item, .embed-responsive iframe, .embed-=
responsive embed, .embed-responsive object, .embed-responsive video { posit=
ion: absolute; top: 0px; bottom: 0px; left: 0px; width: 100%; height: 100%;=
 border: 0px; }

.embed-responsive-16by9 { padding-bottom: 56.25%; }

.embed-responsive-4by3 { padding-bottom: 75%; }

.well { min-height: 20px; padding: 19px; margin-bottom: 20px; background-co=
lor: rgb(245, 245, 245); border: 1px solid rgb(227, 227, 227); border-radiu=
s: 2px; box-shadow: rgba(0, 0, 0, 0.05) 0px 1px 1px inset; }

.well blockquote { border-color: rgba(0, 0, 0, 0.15); }

.well-lg { padding: 24px; border-radius: 3px; }

.well-sm { padding: 9px; border-radius: 1px; }

.close { float: right; font-size: 19.5px; font-weight: bold; line-height: 1=
; color: rgb(0, 0, 0); text-shadow: rgb(255, 255, 255) 0px 1px 0px; opacity=
: 0.2; }

.close:hover, .close:focus { color: rgb(0, 0, 0); text-decoration: none; cu=
rsor: pointer; opacity: 0.5; }

button.close { padding: 0px; cursor: pointer; background: transparent; bord=
er: 0px; appearance: none; }

.modal-open { overflow: hidden; }

.modal { position: fixed; inset: 0px; z-index: 1050; display: none; overflo=
w: hidden; outline: 0px; }

.modal.fade .modal-dialog { transform: translate(0px, -25%); transition: tr=
ansform 0.3s ease-out 0s; }

.modal.in .modal-dialog { transform: translate(0px, 0px); }

.modal-open .modal { overflow: hidden auto; }

.modal-dialog { position: relative; width: auto; margin: 10px; }

.modal-content { position: relative; background-color: rgb(255, 255, 255); =
background-clip: padding-box; border: 1px solid rgba(0, 0, 0, 0.2); border-=
radius: 3px; box-shadow: rgba(0, 0, 0, 0.5) 0px 3px 9px; outline: 0px; }

.modal-backdrop { position: fixed; inset: 0px; z-index: 1040; background-co=
lor: rgb(0, 0, 0); }

.modal-backdrop.fade { opacity: 0; }

.modal-backdrop.in { opacity: 0.5; }

.modal-header { padding: 15px; border-bottom: 1px solid rgb(229, 229, 229);=
 }

.modal-header .close { margin-top: -2px; }

.modal-title { margin: 0px; line-height: 1.42857; }

.modal-body { position: relative; padding: 15px; }

.modal-footer { padding: 15px; text-align: right; border-top: 1px solid rgb=
(229, 229, 229); }

.modal-footer .btn + .btn { margin-bottom: 0px; margin-left: 5px; }

.modal-footer .btn-group .btn + .btn { margin-left: -1px; }

.modal-footer .btn-block + .btn-block { margin-left: 0px; }

.modal-scrollbar-measure { position: absolute; top: -9999px; width: 50px; h=
eight: 50px; overflow: scroll; }

@media (min-width: 768px) {
  .modal-dialog { width: 600px; margin: 30px auto; }
  .modal-content { box-shadow: rgba(0, 0, 0, 0.5) 0px 5px 15px; }
  .modal-sm { width: 300px; }
}

@media (min-width: 992px) {
  .modal-lg { width: 900px; }
}

.tooltip { position: absolute; z-index: 1070; display: block; font-family: =
"Helvetica Neue", Helvetica, Arial, sans-serif; font-style: normal; font-we=
ight: 400; line-height: 1.42857; line-break: auto; text-align: start; text-=
decoration: none; text-shadow: none; text-transform: none; letter-spacing: =
normal; word-break: normal; word-spacing: normal; overflow-wrap: normal; wh=
ite-space: normal; font-size: 12px; opacity: 0; }

.tooltip.in { opacity: 0.9; }

.tooltip.top { padding: 5px 0px; margin-top: -3px; }

.tooltip.right { padding: 0px 5px; margin-left: 3px; }

.tooltip.bottom { padding: 5px 0px; margin-top: 3px; }

.tooltip.left { padding: 0px 5px; margin-left: -3px; }

.tooltip.top .tooltip-arrow { bottom: 0px; left: 50%; margin-left: -5px; bo=
rder-width: 5px 5px 0px; border-top-color: rgb(0, 0, 0); }

.tooltip.top-left .tooltip-arrow { right: 5px; bottom: 0px; margin-bottom: =
-5px; border-width: 5px 5px 0px; border-top-color: rgb(0, 0, 0); }

.tooltip.top-right .tooltip-arrow { bottom: 0px; left: 5px; margin-bottom: =
-5px; border-width: 5px 5px 0px; border-top-color: rgb(0, 0, 0); }

.tooltip.right .tooltip-arrow { top: 50%; left: 0px; margin-top: -5px; bord=
er-width: 5px 5px 5px 0px; border-right-color: rgb(0, 0, 0); }

.tooltip.left .tooltip-arrow { top: 50%; right: 0px; margin-top: -5px; bord=
er-width: 5px 0px 5px 5px; border-left-color: rgb(0, 0, 0); }

.tooltip.bottom .tooltip-arrow { top: 0px; left: 50%; margin-left: -5px; bo=
rder-width: 0px 5px 5px; border-bottom-color: rgb(0, 0, 0); }

.tooltip.bottom-left .tooltip-arrow { top: 0px; right: 5px; margin-top: -5p=
x; border-width: 0px 5px 5px; border-bottom-color: rgb(0, 0, 0); }

.tooltip.bottom-right .tooltip-arrow { top: 0px; left: 5px; margin-top: -5p=
x; border-width: 0px 5px 5px; border-bottom-color: rgb(0, 0, 0); }

.tooltip-inner { max-width: 200px; padding: 3px 8px; color: rgb(255, 255, 2=
55); text-align: center; background-color: rgb(0, 0, 0); border-radius: 2px=
; }

.tooltip-arrow { position: absolute; width: 0px; height: 0px; border-color:=
 transparent; border-style: solid; }

.popover { position: absolute; top: 0px; left: 0px; z-index: 1060; display:=
 none; max-width: 276px; padding: 1px; font-family: "Helvetica Neue", Helve=
tica, Arial, sans-serif; font-style: normal; font-weight: 400; line-height:=
 1.42857; line-break: auto; text-align: start; text-decoration: none; text-=
shadow: none; text-transform: none; letter-spacing: normal; word-break: nor=
mal; word-spacing: normal; overflow-wrap: normal; white-space: normal; font=
-size: 13px; background-color: rgb(255, 255, 255); background-clip: padding=
-box; border: 1px solid rgba(0, 0, 0, 0.2); border-radius: 3px; box-shadow:=
 rgba(0, 0, 0, 0.2) 0px 5px 10px; }

.popover.top { margin-top: -10px; }

.popover.right { margin-left: 10px; }

.popover.bottom { margin-top: 10px; }

.popover.left { margin-left: -10px; }

.popover > .arrow { border-width: 11px; }

.popover > .arrow, .popover > .arrow::after { position: absolute; display: =
block; width: 0px; height: 0px; border-color: transparent; border-style: so=
lid; }

.popover > .arrow::after { content: ""; border-width: 10px; }

.popover.top > .arrow { bottom: -11px; left: 50%; margin-left: -11px; borde=
r-top-color: rgba(0, 0, 0, 0.25); border-bottom-width: 0px; }

.popover.top > .arrow::after { bottom: 1px; margin-left: -10px; content: " =
"; border-top-color: rgb(255, 255, 255); border-bottom-width: 0px; }

.popover.right > .arrow { top: 50%; left: -11px; margin-top: -11px; border-=
right-color: rgba(0, 0, 0, 0.25); border-left-width: 0px; }

.popover.right > .arrow::after { bottom: -10px; left: 1px; content: " "; bo=
rder-right-color: rgb(255, 255, 255); border-left-width: 0px; }

.popover.bottom > .arrow { top: -11px; left: 50%; margin-left: -11px; borde=
r-top-width: 0px; border-bottom-color: rgba(0, 0, 0, 0.25); }

.popover.bottom > .arrow::after { top: 1px; margin-left: -10px; content: " =
"; border-top-width: 0px; border-bottom-color: rgb(255, 255, 255); }

.popover.left > .arrow { top: 50%; right: -11px; margin-top: -11px; border-=
right-width: 0px; border-left-color: rgba(0, 0, 0, 0.25); }

.popover.left > .arrow::after { right: 1px; bottom: -10px; content: " "; bo=
rder-right-width: 0px; border-left-color: rgb(255, 255, 255); }

.popover-title { padding: 8px 14px; margin: 0px; font-size: 13px; backgroun=
d-color: rgb(247, 247, 247); border-bottom: 1px solid rgb(235, 235, 235); b=
order-radius: 2px 2px 0px 0px; }

.popover-content { padding: 9px 14px; }

.carousel { position: relative; }

.carousel-inner { position: relative; width: 100%; overflow: hidden; }

.carousel-inner > .item { position: relative; display: none; transition: le=
ft 0.6s ease-in-out 0s; }

.carousel-inner > .item > img, .carousel-inner > .item > a > img { line-hei=
ght: 1; }

@media (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item { transition: transform 0.6s ease-in-out 0s; back=
face-visibility: hidden; perspective: 1000px; }
  .carousel-inner > .item.next, .carousel-inner > .item.active.right { tran=
sform: translate3d(100%, 0px, 0px); left: 0px; }
  .carousel-inner > .item.prev, .carousel-inner > .item.active.left { trans=
form: translate3d(-100%, 0px, 0px); left: 0px; }
  .carousel-inner > .item.next.left, .carousel-inner > .item.prev.right, .c=
arousel-inner > .item.active { transform: translate3d(0px, 0px, 0px); left:=
 0px; }
}

.carousel-inner > .active, .carousel-inner > .next, .carousel-inner > .prev=
 { display: block; }

.carousel-inner > .active { left: 0px; }

.carousel-inner > .next, .carousel-inner > .prev { position: absolute; top:=
 0px; width: 100%; }

.carousel-inner > .next { left: 100%; }

.carousel-inner > .prev { left: -100%; }

.carousel-inner > .next.left, .carousel-inner > .prev.right { left: 0px; }

.carousel-inner > .active.left { left: -100%; }

.carousel-inner > .active.right { left: 100%; }

.carousel-control { position: absolute; top: 0px; bottom: 0px; left: 0px; w=
idth: 15%; font-size: 20px; color: rgb(255, 255, 255); text-align: center; =
text-shadow: rgba(0, 0, 0, 0.6) 0px 1px 2px; background-color: rgba(0, 0, 0=
, 0); opacity: 0.5; }

.carousel-control.left { background-image: linear-gradient(to right, rgba(0=
, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0) 100%); background-repeat: repeat-x; }

.carousel-control.right { right: 0px; left: auto; background-image: linear-=
gradient(to right, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.5) 100%); backgroun=
d-repeat: repeat-x; }

.carousel-control:hover, .carousel-control:focus { color: rgb(255, 255, 255=
); text-decoration: none; outline: 0px; opacity: 0.9; }

.carousel-control .icon-prev, .carousel-control .icon-next, .carousel-contr=
ol .glyphicon-chevron-left, .carousel-control .glyphicon-chevron-right { po=
sition: absolute; top: 50%; z-index: 5; display: inline-block; margin-top: =
-10px; }

.carousel-control .icon-prev, .carousel-control .glyphicon-chevron-left { l=
eft: 50%; margin-left: -10px; }

.carousel-control .icon-next, .carousel-control .glyphicon-chevron-right { =
right: 50%; margin-right: -10px; }

.carousel-control .icon-prev, .carousel-control .icon-next { width: 20px; h=
eight: 20px; font-family: serif; line-height: 1; }

.carousel-control .icon-prev::before { content: "=E2=80=B9"; }

.carousel-control .icon-next::before { content: "=E2=80=BA"; }

.carousel-indicators { position: absolute; bottom: 10px; left: 50%; z-index=
: 15; width: 60%; padding-left: 0px; margin-left: -30%; text-align: center;=
 list-style: none; }

.carousel-indicators li { display: inline-block; width: 10px; height: 10px;=
 margin: 1px; text-indent: -999px; cursor: pointer; background-color: rgba(=
0, 0, 0, 0); border: 1px solid rgb(255, 255, 255); border-radius: 10px; }

.carousel-indicators .active { width: 12px; height: 12px; margin: 0px; back=
ground-color: rgb(255, 255, 255); }

.carousel-caption { position: absolute; right: 15%; bottom: 20px; left: 15%=
; z-index: 10; padding-top: 20px; padding-bottom: 20px; color: rgb(255, 255=
, 255); text-align: center; text-shadow: rgba(0, 0, 0, 0.6) 0px 1px 2px; }

.carousel-caption .btn { text-shadow: none; }

@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left, .carousel-control .glyphicon-c=
hevron-right, .carousel-control .icon-prev, .carousel-control .icon-next { =
width: 30px; height: 30px; margin-top: -10px; font-size: 30px; }
  .carousel-control .glyphicon-chevron-left, .carousel-control .icon-prev {=
 margin-left: -10px; }
  .carousel-control .glyphicon-chevron-right, .carousel-control .icon-next =
{ margin-right: -10px; }
  .carousel-caption { right: 20%; left: 20%; padding-bottom: 30px; }
  .carousel-indicators { bottom: 20px; }
}

.clearfix::before, .clearfix::after, .dl-horizontal dd::before, .dl-horizon=
tal dd::after, .container::before, .container::after, .container-fluid::bef=
ore, .container-fluid::after, .row::before, .row::after, .form-horizontal .=
form-group::before, .form-horizontal .form-group::after, .btn-toolbar::befo=
re, .btn-toolbar::after, .btn-group-vertical > .btn-group::before, .btn-gro=
up-vertical > .btn-group::after, .nav::before, .nav::after, .navbar::before=
, .navbar::after, .navbar-header::before, .navbar-header::after, .navbar-co=
llapse::before, .navbar-collapse::after, .pager::before, .pager::after, .pa=
nel-body::before, .panel-body::after, .modal-header::before, .modal-header:=
:after, .modal-footer::before, .modal-footer::after, .item_buttons::before,=
 .item_buttons::after { display: table; content: " "; }

.clearfix::after, .dl-horizontal dd::after, .container::after, .container-f=
luid::after, .row::after, .form-horizontal .form-group::after, .btn-toolbar=
::after, .btn-group-vertical > .btn-group::after, .nav::after, .navbar::aft=
er, .navbar-header::after, .navbar-collapse::after, .pager::after, .panel-b=
ody::after, .modal-header::after, .modal-footer::after, .item_buttons::afte=
r { clear: both; }

.center-block { display: block; margin-right: auto; margin-left: auto; }

.pull-right { float: right !important; }

.pull-left { float: left !important; }

.hide { display: none !important; }

.show { display: block !important; }

.invisible { visibility: hidden; }

.text-hide { font: 0px / 0 a; color: transparent; text-shadow: none; backgr=
ound-color: transparent; border: 0px; }

.hidden { display: none !important; }

.affix { position: fixed; }

.visible-xs, .visible-sm, .visible-md, .visible-lg { display: none !importa=
nt; }

.visible-xs-block, .visible-xs-inline, .visible-xs-inline-block, .visible-s=
m-block, .visible-sm-inline, .visible-sm-inline-block, .visible-md-block, .=
visible-md-inline, .visible-md-inline-block, .visible-lg-block, .visible-lg=
-inline, .visible-lg-inline-block { display: none !important; }

@media (max-width: 767px) {
  .visible-xs { display: block !important; }
  table.visible-xs { display: table !important; }
  tr.visible-xs { display: table-row !important; }
  th.visible-xs, td.visible-xs { display: table-cell !important; }
}

@media (max-width: 767px) {
  .visible-xs-block { display: block !important; }
}

@media (max-width: 767px) {
  .visible-xs-inline { display: inline !important; }
}

@media (max-width: 767px) {
  .visible-xs-inline-block { display: inline-block !important; }
}

@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm { display: block !important; }
  table.visible-sm { display: table !important; }
  tr.visible-sm { display: table-row !important; }
  th.visible-sm, td.visible-sm { display: table-cell !important; }
}

@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block { display: block !important; }
}

@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline { display: inline !important; }
}

@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block { display: inline-block !important; }
}

@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md { display: block !important; }
  table.visible-md { display: table !important; }
  tr.visible-md { display: table-row !important; }
  th.visible-md, td.visible-md { display: table-cell !important; }
}

@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block { display: block !important; }
}

@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline { display: inline !important; }
}

@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block { display: inline-block !important; }
}

@media (min-width: 1200px) {
  .visible-lg { display: block !important; }
  table.visible-lg { display: table !important; }
  tr.visible-lg { display: table-row !important; }
  th.visible-lg, td.visible-lg { display: table-cell !important; }
}

@media (min-width: 1200px) {
  .visible-lg-block { display: block !important; }
}

@media (min-width: 1200px) {
  .visible-lg-inline { display: inline !important; }
}

@media (min-width: 1200px) {
  .visible-lg-inline-block { display: inline-block !important; }
}

@media (max-width: 767px) {
  .hidden-xs { display: none !important; }
}

@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm { display: none !important; }
}

@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md { display: none !important; }
}

@media (min-width: 1200px) {
  .hidden-lg { display: none !important; }
}

.visible-print { display: none !important; }

@media print {
  .visible-print { display: block !important; }
  table.visible-print { display: table !important; }
  tr.visible-print { display: table-row !important; }
  th.visible-print, td.visible-print { display: table-cell !important; }
}

.visible-print-block { display: none !important; }

@media print {
  .visible-print-block { display: block !important; }
}

.visible-print-inline { display: none !important; }

@media print {
  .visible-print-inline { display: inline !important; }
}

.visible-print-inline-block { display: none !important; }

@media print {
  .visible-print-inline-block { display: inline-block !important; }
}

@media print {
  .hidden-print { display: none !important; }
}

@font-face { font-family: FontAwesome; src: url("../components/font-awesome=
/fonts/fontawesome-webfont.woff2?v=3D4.7.0") format("woff2"), url("../compo=
nents/font-awesome/fonts/fontawesome-webfont.woff?v=3D4.7.0") format("woff"=
), url("../components/font-awesome/fonts/fontawesome-webfont.ttf?v=3D4.7.0"=
) format("truetype"); font-weight: normal; font-style: normal; }

.fa { display: inline-block; font-style: normal; font-variant: normal; font=
-kerning: auto; font-optical-sizing: auto; font-feature-settings: normal; f=
ont-variation-settings: normal; font-weight: normal; font-stretch: normal; =
line-height: 1; font-family: FontAwesome; font-size: inherit; text-renderin=
g: auto; -webkit-font-smoothing: antialiased; }

.fa-lg { font-size: 1.33333em; line-height: 0.75em; vertical-align: -15%; }

.fa-2x { font-size: 2em; }

.fa-3x { font-size: 3em; }

.fa-4x { font-size: 4em; }

.fa-5x { font-size: 5em; }

.fa-fw { width: 1.28571em; text-align: center; }

.fa-ul { padding-left: 0px; margin-left: 2.14286em; list-style-type: none; =
}

.fa-ul > li { position: relative; }

.fa-li { position: absolute; left: -2.14286em; width: 2.14286em; top: 0.142=
857em; text-align: center; }

.fa-li.fa-lg { left: -1.85714em; }

.fa-border { padding: 0.2em 0.25em 0.15em; border: 0.08em solid rgb(238, 23=
8, 238); border-radius: 0.1em; }

.fa-pull-left { float: left; }

.fa-pull-right { float: right; }

.fa.fa-pull-left { margin-right: 0.3em; }

.fa.fa-pull-right { margin-left: 0.3em; }

.pull-right { float: right; }

.pull-left { float: left; }

.fa.pull-left { margin-right: 0.3em; }

.fa.pull-right { margin-left: 0.3em; }

.fa-spin { animation: 2s linear 0s infinite normal none running fa-spin; }

.fa-pulse { animation: 1s steps(8) 0s infinite normal none running fa-spin;=
 }

@-webkit-keyframes fa-spin {=20
  0% { transform: rotate(0deg); }
  100% { transform: rotate(359deg); }
}

@keyframes fa-spin {=20
  0% { transform: rotate(0deg); }
  100% { transform: rotate(359deg); }
}

.fa-rotate-90 { transform: rotate(90deg); }

.fa-rotate-180 { transform: rotate(180deg); }

.fa-rotate-270 { transform: rotate(270deg); }

.fa-flip-horizontal { transform: scale(-1, 1); }

.fa-flip-vertical { transform: scale(1, -1); }

:root .fa-rotate-90, :root .fa-rotate-180, :root .fa-rotate-270, :root .fa-=
flip-horizontal, :root .fa-flip-vertical { filter: none; }

.fa-stack { position: relative; display: inline-block; width: 2em; height: =
2em; line-height: 2em; vertical-align: middle; }

.fa-stack-1x, .fa-stack-2x { position: absolute; left: 0px; width: 100%; te=
xt-align: center; }

.fa-stack-1x { line-height: inherit; }

.fa-stack-2x { font-size: 2em; }

.fa-inverse { color: rgb(255, 255, 255); }

.fa-glass::before { content: "=EF=80=80"; }

.fa-music::before { content: "=EF=80=81"; }

.fa-search::before { content: "=EF=80=82"; }

.fa-envelope-o::before { content: "=EF=80=83"; }

.fa-heart::before { content: "=EF=80=84"; }

.fa-star::before { content: "=EF=80=85"; }

.fa-star-o::before { content: "=EF=80=86"; }

.fa-user::before { content: "=EF=80=87"; }

.fa-film::before { content: "=EF=80=88"; }

.fa-th-large::before { content: "=EF=80=89"; }

.fa-th::before { content: "=EF=80=8A"; }

.fa-th-list::before { content: "=EF=80=8B"; }

.fa-check::before { content: "=EF=80=8C"; }

.fa-remove::before, .fa-close::before, .fa-times::before { content: "=EF=80=
=8D"; }

.fa-search-plus::before { content: "=EF=80=8E"; }

.fa-search-minus::before { content: "=EF=80=90"; }

.fa-power-off::before { content: "=EF=80=91"; }

.fa-signal::before { content: "=EF=80=92"; }

.fa-gear::before, .fa-cog::before { content: "=EF=80=93"; }

.fa-trash-o::before { content: "=EF=80=94"; }

.fa-home::before { content: "=EF=80=95"; }

.fa-file-o::before { content: "=EF=80=96"; }

.fa-clock-o::before { content: "=EF=80=97"; }

.fa-road::before { content: "=EF=80=98"; }

.fa-download::before { content: "=EF=80=99"; }

.fa-arrow-circle-o-down::before { content: "=EF=80=9A"; }

.fa-arrow-circle-o-up::before { content: "=EF=80=9B"; }

.fa-inbox::before { content: "=EF=80=9C"; }

.fa-play-circle-o::before { content: "=EF=80=9D"; }

.fa-rotate-right::before, .fa-repeat::before { content: "=EF=80=9E"; }

.fa-refresh::before { content: "=EF=80=A1"; }

.fa-list-alt::before { content: "=EF=80=A2"; }

.fa-lock::before { content: "=EF=80=A3"; }

.fa-flag::before { content: "=EF=80=A4"; }

.fa-headphones::before { content: "=EF=80=A5"; }

.fa-volume-off::before { content: "=EF=80=A6"; }

.fa-volume-down::before { content: "=EF=80=A7"; }

.fa-volume-up::before { content: "=EF=80=A8"; }

.fa-qrcode::before { content: "=EF=80=A9"; }

.fa-barcode::before { content: "=EF=80=AA"; }

.fa-tag::before { content: "=EF=80=AB"; }

.fa-tags::before { content: "=EF=80=AC"; }

.fa-book::before { content: "=EF=80=AD"; }

.fa-bookmark::before { content: "=EF=80=AE"; }

.fa-print::before { content: "=EF=80=AF"; }

.fa-camera::before { content: "=EF=80=B0"; }

.fa-font::before { content: "=EF=80=B1"; }

.fa-bold::before { content: "=EF=80=B2"; }

.fa-italic::before { content: "=EF=80=B3"; }

.fa-text-height::before { content: "=EF=80=B4"; }

.fa-text-width::before { content: "=EF=80=B5"; }

.fa-align-left::before { content: "=EF=80=B6"; }

.fa-align-center::before { content: "=EF=80=B7"; }

.fa-align-right::before { content: "=EF=80=B8"; }

.fa-align-justify::before { content: "=EF=80=B9"; }

.fa-list::before { content: "=EF=80=BA"; }

.fa-dedent::before, .fa-outdent::before { content: "=EF=80=BB"; }

.fa-indent::before { content: "=EF=80=BC"; }

.fa-video-camera::before { content: "=EF=80=BD"; }

.fa-photo::before, .fa-image::before, .fa-picture-o::before { content: "=EF=
=80=BE"; }

.fa-pencil::before { content: "=EF=81=80"; }

.fa-map-marker::before { content: "=EF=81=81"; }

.fa-adjust::before { content: "=EF=81=82"; }

.fa-tint::before { content: "=EF=81=83"; }

.fa-edit::before, .fa-pencil-square-o::before { content: "=EF=81=84"; }

.fa-share-square-o::before { content: "=EF=81=85"; }

.fa-check-square-o::before { content: "=EF=81=86"; }

.fa-arrows::before { content: "=EF=81=87"; }

.fa-step-backward::before { content: "=EF=81=88"; }

.fa-fast-backward::before { content: "=EF=81=89"; }

.fa-backward::before { content: "=EF=81=8A"; }

.fa-play::before { content: "=EF=81=8B"; }

.fa-pause::before { content: "=EF=81=8C"; }

.fa-stop::before { content: "=EF=81=8D"; }

.fa-forward::before { content: "=EF=81=8E"; }

.fa-fast-forward::before { content: "=EF=81=90"; }

.fa-step-forward::before { content: "=EF=81=91"; }

.fa-eject::before { content: "=EF=81=92"; }

.fa-chevron-left::before { content: "=EF=81=93"; }

.fa-chevron-right::before { content: "=EF=81=94"; }

.fa-plus-circle::before { content: "=EF=81=95"; }

.fa-minus-circle::before { content: "=EF=81=96"; }

.fa-times-circle::before { content: "=EF=81=97"; }

.fa-check-circle::before { content: "=EF=81=98"; }

.fa-question-circle::before { content: "=EF=81=99"; }

.fa-info-circle::before { content: "=EF=81=9A"; }

.fa-crosshairs::before { content: "=EF=81=9B"; }

.fa-times-circle-o::before { content: "=EF=81=9C"; }

.fa-check-circle-o::before { content: "=EF=81=9D"; }

.fa-ban::before { content: "=EF=81=9E"; }

.fa-arrow-left::before { content: "=EF=81=A0"; }

.fa-arrow-right::before { content: "=EF=81=A1"; }

.fa-arrow-up::before { content: "=EF=81=A2"; }

.fa-arrow-down::before { content: "=EF=81=A3"; }

.fa-mail-forward::before, .fa-share::before { content: "=EF=81=A4"; }

.fa-expand::before { content: "=EF=81=A5"; }

.fa-compress::before { content: "=EF=81=A6"; }

.fa-plus::before { content: "=EF=81=A7"; }

.fa-minus::before { content: "=EF=81=A8"; }

.fa-asterisk::before { content: "=EF=81=A9"; }

.fa-exclamation-circle::before { content: "=EF=81=AA"; }

.fa-gift::before { content: "=EF=81=AB"; }

.fa-leaf::before { content: "=EF=81=AC"; }

.fa-fire::before { content: "=EF=81=AD"; }

.fa-eye::before { content: "=EF=81=AE"; }

.fa-eye-slash::before { content: "=EF=81=B0"; }

.fa-warning::before, .fa-exclamation-triangle::before { content: "=EF=81=B1=
"; }

.fa-plane::before { content: "=EF=81=B2"; }

.fa-calendar::before { content: "=EF=81=B3"; }

.fa-random::before { content: "=EF=81=B4"; }

.fa-comment::before { content: "=EF=81=B5"; }

.fa-magnet::before { content: "=EF=81=B6"; }

.fa-chevron-up::before { content: "=EF=81=B7"; }

.fa-chevron-down::before { content: "=EF=81=B8"; }

.fa-retweet::before { content: "=EF=81=B9"; }

.fa-shopping-cart::before { content: "=EF=81=BA"; }

.fa-folder::before { content: "=EF=81=BB"; }

.fa-folder-open::before { content: "=EF=81=BC"; }

.fa-arrows-v::before { content: "=EF=81=BD"; }

.fa-arrows-h::before { content: "=EF=81=BE"; }

.fa-bar-chart-o::before, .fa-bar-chart::before { content: "=EF=82=80"; }

.fa-twitter-square::before { content: "=EF=82=81"; }

.fa-facebook-square::before { content: "=EF=82=82"; }

.fa-camera-retro::before { content: "=EF=82=83"; }

.fa-key::before { content: "=EF=82=84"; }

.fa-gears::before, .fa-cogs::before { content: "=EF=82=85"; }

.fa-comments::before { content: "=EF=82=86"; }

.fa-thumbs-o-up::before { content: "=EF=82=87"; }

.fa-thumbs-o-down::before { content: "=EF=82=88"; }

.fa-star-half::before { content: "=EF=82=89"; }

.fa-heart-o::before { content: "=EF=82=8A"; }

.fa-sign-out::before { content: "=EF=82=8B"; }

.fa-linkedin-square::before { content: "=EF=82=8C"; }

.fa-thumb-tack::before { content: "=EF=82=8D"; }

.fa-external-link::before { content: "=EF=82=8E"; }

.fa-sign-in::before { content: "=EF=82=90"; }

.fa-trophy::before { content: "=EF=82=91"; }

.fa-github-square::before { content: "=EF=82=92"; }

.fa-upload::before { content: "=EF=82=93"; }

.fa-lemon-o::before { content: "=EF=82=94"; }

.fa-phone::before { content: "=EF=82=95"; }

.fa-square-o::before { content: "=EF=82=96"; }

.fa-bookmark-o::before { content: "=EF=82=97"; }

.fa-phone-square::before { content: "=EF=82=98"; }

.fa-twitter::before { content: "=EF=82=99"; }

.fa-facebook-f::before, .fa-facebook::before { content: "=EF=82=9A"; }

.fa-github::before { content: "=EF=82=9B"; }

.fa-unlock::before { content: "=EF=82=9C"; }

.fa-credit-card::before { content: "=EF=82=9D"; }

.fa-feed::before, .fa-rss::before { content: "=EF=82=9E"; }

.fa-hdd-o::before { content: "=EF=82=A0"; }

.fa-bullhorn::before { content: "=EF=82=A1"; }

.fa-bell::before { content: "=EF=83=B3"; }

.fa-certificate::before { content: "=EF=82=A3"; }

.fa-hand-o-right::before { content: "=EF=82=A4"; }

.fa-hand-o-left::before { content: "=EF=82=A5"; }

.fa-hand-o-up::before { content: "=EF=82=A6"; }

.fa-hand-o-down::before { content: "=EF=82=A7"; }

.fa-arrow-circle-left::before { content: "=EF=82=A8"; }

.fa-arrow-circle-right::before { content: "=EF=82=A9"; }

.fa-arrow-circle-up::before { content: "=EF=82=AA"; }

.fa-arrow-circle-down::before { content: "=EF=82=AB"; }

.fa-globe::before { content: "=EF=82=AC"; }

.fa-wrench::before { content: "=EF=82=AD"; }

.fa-tasks::before { content: "=EF=82=AE"; }

.fa-filter::before { content: "=EF=82=B0"; }

.fa-briefcase::before { content: "=EF=82=B1"; }

.fa-arrows-alt::before { content: "=EF=82=B2"; }

.fa-group::before, .fa-users::before { content: "=EF=83=80"; }

.fa-chain::before, .fa-link::before { content: "=EF=83=81"; }

.fa-cloud::before { content: "=EF=83=82"; }

.fa-flask::before { content: "=EF=83=83"; }

.fa-cut::before, .fa-scissors::before { content: "=EF=83=84"; }

.fa-copy::before, .fa-files-o::before { content: "=EF=83=85"; }

.fa-paperclip::before { content: "=EF=83=86"; }

.fa-save::before, .fa-floppy-o::before { content: "=EF=83=87"; }

.fa-square::before { content: "=EF=83=88"; }

.fa-navicon::before, .fa-reorder::before, .fa-bars::before { content: "=EF=
=83=89"; }

.fa-list-ul::before { content: "=EF=83=8A"; }

.fa-list-ol::before { content: "=EF=83=8B"; }

.fa-strikethrough::before { content: "=EF=83=8C"; }

.fa-underline::before { content: "=EF=83=8D"; }

.fa-table::before { content: "=EF=83=8E"; }

.fa-magic::before { content: "=EF=83=90"; }

.fa-truck::before { content: "=EF=83=91"; }

.fa-pinterest::before { content: "=EF=83=92"; }

.fa-pinterest-square::before { content: "=EF=83=93"; }

.fa-google-plus-square::before { content: "=EF=83=94"; }

.fa-google-plus::before { content: "=EF=83=95"; }

.fa-money::before { content: "=EF=83=96"; }

.fa-caret-down::before { content: "=EF=83=97"; }

.fa-caret-up::before { content: "=EF=83=98"; }

.fa-caret-left::before { content: "=EF=83=99"; }

.fa-caret-right::before { content: "=EF=83=9A"; }

.fa-columns::before { content: "=EF=83=9B"; }

.fa-unsorted::before, .fa-sort::before { content: "=EF=83=9C"; }

.fa-sort-down::before, .fa-sort-desc::before { content: "=EF=83=9D"; }

.fa-sort-up::before, .fa-sort-asc::before { content: "=EF=83=9E"; }

.fa-envelope::before { content: "=EF=83=A0"; }

.fa-linkedin::before { content: "=EF=83=A1"; }

.fa-rotate-left::before, .fa-undo::before { content: "=EF=83=A2"; }

.fa-legal::before, .fa-gavel::before { content: "=EF=83=A3"; }

.fa-dashboard::before, .fa-tachometer::before { content: "=EF=83=A4"; }

.fa-comment-o::before { content: "=EF=83=A5"; }

.fa-comments-o::before { content: "=EF=83=A6"; }

.fa-flash::before, .fa-bolt::before { content: "=EF=83=A7"; }

.fa-sitemap::before { content: "=EF=83=A8"; }

.fa-umbrella::before { content: "=EF=83=A9"; }

.fa-paste::before, .fa-clipboard::before { content: "=EF=83=AA"; }

.fa-lightbulb-o::before { content: "=EF=83=AB"; }

.fa-exchange::before { content: "=EF=83=AC"; }

.fa-cloud-download::before { content: "=EF=83=AD"; }

.fa-cloud-upload::before { content: "=EF=83=AE"; }

.fa-user-md::before { content: "=EF=83=B0"; }

.fa-stethoscope::before { content: "=EF=83=B1"; }

.fa-suitcase::before { content: "=EF=83=B2"; }

.fa-bell-o::before { content: "=EF=82=A2"; }

.fa-coffee::before { content: "=EF=83=B4"; }

.fa-cutlery::before { content: "=EF=83=B5"; }

.fa-file-text-o::before { content: "=EF=83=B6"; }

.fa-building-o::before { content: "=EF=83=B7"; }

.fa-hospital-o::before { content: "=EF=83=B8"; }

.fa-ambulance::before { content: "=EF=83=B9"; }

.fa-medkit::before { content: "=EF=83=BA"; }

.fa-fighter-jet::before { content: "=EF=83=BB"; }

.fa-beer::before { content: "=EF=83=BC"; }

.fa-h-square::before { content: "=EF=83=BD"; }

.fa-plus-square::before { content: "=EF=83=BE"; }

.fa-angle-double-left::before { content: "=EF=84=80"; }

.fa-angle-double-right::before { content: "=EF=84=81"; }

.fa-angle-double-up::before { content: "=EF=84=82"; }

.fa-angle-double-down::before { content: "=EF=84=83"; }

.fa-angle-left::before { content: "=EF=84=84"; }

.fa-angle-right::before { content: "=EF=84=85"; }

.fa-angle-up::before { content: "=EF=84=86"; }

.fa-angle-down::before { content: "=EF=84=87"; }

.fa-desktop::before { content: "=EF=84=88"; }

.fa-laptop::before { content: "=EF=84=89"; }

.fa-tablet::before { content: "=EF=84=8A"; }

.fa-mobile-phone::before, .fa-mobile::before { content: "=EF=84=8B"; }

.fa-circle-o::before { content: "=EF=84=8C"; }

.fa-quote-left::before { content: "=EF=84=8D"; }

.fa-quote-right::before { content: "=EF=84=8E"; }

.fa-spinner::before { content: "=EF=84=90"; }

.fa-circle::before { content: "=EF=84=91"; }

.fa-mail-reply::before, .fa-reply::before { content: "=EF=84=92"; }

.fa-github-alt::before { content: "=EF=84=93"; }

.fa-folder-o::before { content: "=EF=84=94"; }

.fa-folder-open-o::before { content: "=EF=84=95"; }

.fa-smile-o::before { content: "=EF=84=98"; }

.fa-frown-o::before { content: "=EF=84=99"; }

.fa-meh-o::before { content: "=EF=84=9A"; }

.fa-gamepad::before { content: "=EF=84=9B"; }

.fa-keyboard-o::before { content: "=EF=84=9C"; }

.fa-flag-o::before { content: "=EF=84=9D"; }

.fa-flag-checkered::before { content: "=EF=84=9E"; }

.fa-terminal::before { content: "=EF=84=A0"; }

.fa-code::before { content: "=EF=84=A1"; }

.fa-mail-reply-all::before, .fa-reply-all::before { content: "=EF=84=A2"; }

.fa-star-half-empty::before, .fa-star-half-full::before, .fa-star-half-o::b=
efore { content: "=EF=84=A3"; }

.fa-location-arrow::before { content: "=EF=84=A4"; }

.fa-crop::before { content: "=EF=84=A5"; }

.fa-code-fork::before { content: "=EF=84=A6"; }

.fa-unlink::before, .fa-chain-broken::before { content: "=EF=84=A7"; }

.fa-question::before { content: "=EF=84=A8"; }

.fa-info::before { content: "=EF=84=A9"; }

.fa-exclamation::before { content: "=EF=84=AA"; }

.fa-superscript::before { content: "=EF=84=AB"; }

.fa-subscript::before { content: "=EF=84=AC"; }

.fa-eraser::before { content: "=EF=84=AD"; }

.fa-puzzle-piece::before { content: "=EF=84=AE"; }

.fa-microphone::before { content: "=EF=84=B0"; }

.fa-microphone-slash::before { content: "=EF=84=B1"; }

.fa-shield::before { content: "=EF=84=B2"; }

.fa-calendar-o::before { content: "=EF=84=B3"; }

.fa-fire-extinguisher::before { content: "=EF=84=B4"; }

.fa-rocket::before { content: "=EF=84=B5"; }

.fa-maxcdn::before { content: "=EF=84=B6"; }

.fa-chevron-circle-left::before { content: "=EF=84=B7"; }

.fa-chevron-circle-right::before { content: "=EF=84=B8"; }

.fa-chevron-circle-up::before { content: "=EF=84=B9"; }

.fa-chevron-circle-down::before { content: "=EF=84=BA"; }

.fa-html5::before { content: "=EF=84=BB"; }

.fa-css3::before { content: "=EF=84=BC"; }

.fa-anchor::before { content: "=EF=84=BD"; }

.fa-unlock-alt::before { content: "=EF=84=BE"; }

.fa-bullseye::before { content: "=EF=85=80"; }

.fa-ellipsis-h::before { content: "=EF=85=81"; }

.fa-ellipsis-v::before { content: "=EF=85=82"; }

.fa-rss-square::before { content: "=EF=85=83"; }

.fa-play-circle::before { content: "=EF=85=84"; }

.fa-ticket::before { content: "=EF=85=85"; }

.fa-minus-square::before { content: "=EF=85=86"; }

.fa-minus-square-o::before { content: "=EF=85=87"; }

.fa-level-up::before { content: "=EF=85=88"; }

.fa-level-down::before { content: "=EF=85=89"; }

.fa-check-square::before { content: "=EF=85=8A"; }

.fa-pencil-square::before { content: "=EF=85=8B"; }

.fa-external-link-square::before { content: "=EF=85=8C"; }

.fa-share-square::before { content: "=EF=85=8D"; }

.fa-compass::before { content: "=EF=85=8E"; }

.fa-toggle-down::before, .fa-caret-square-o-down::before { content: "=EF=85=
=90"; }

.fa-toggle-up::before, .fa-caret-square-o-up::before { content: "=EF=85=91"=
; }

.fa-toggle-right::before, .fa-caret-square-o-right::before { content: "=EF=
=85=92"; }

.fa-euro::before, .fa-eur::before { content: "=EF=85=93"; }

.fa-gbp::before { content: "=EF=85=94"; }

.fa-dollar::before, .fa-usd::before { content: "=EF=85=95"; }

.fa-rupee::before, .fa-inr::before { content: "=EF=85=96"; }

.fa-cny::before, .fa-rmb::before, .fa-yen::before, .fa-jpy::before { conten=
t: "=EF=85=97"; }

.fa-ruble::before, .fa-rouble::before, .fa-rub::before { content: "=EF=85=
=98"; }

.fa-won::before, .fa-krw::before { content: "=EF=85=99"; }

.fa-bitcoin::before, .fa-btc::before { content: "=EF=85=9A"; }

.fa-file::before { content: "=EF=85=9B"; }

.fa-file-text::before { content: "=EF=85=9C"; }

.fa-sort-alpha-asc::before { content: "=EF=85=9D"; }

.fa-sort-alpha-desc::before { content: "=EF=85=9E"; }

.fa-sort-amount-asc::before { content: "=EF=85=A0"; }

.fa-sort-amount-desc::before { content: "=EF=85=A1"; }

.fa-sort-numeric-asc::before { content: "=EF=85=A2"; }

.fa-sort-numeric-desc::before { content: "=EF=85=A3"; }

.fa-thumbs-up::before { content: "=EF=85=A4"; }

.fa-thumbs-down::before { content: "=EF=85=A5"; }

.fa-youtube-square::before { content: "=EF=85=A6"; }

.fa-youtube::before { content: "=EF=85=A7"; }

.fa-xing::before { content: "=EF=85=A8"; }

.fa-xing-square::before { content: "=EF=85=A9"; }

.fa-youtube-play::before { content: "=EF=85=AA"; }

.fa-dropbox::before { content: "=EF=85=AB"; }

.fa-stack-overflow::before { content: "=EF=85=AC"; }

.fa-instagram::before { content: "=EF=85=AD"; }

.fa-flickr::before { content: "=EF=85=AE"; }

.fa-adn::before { content: "=EF=85=B0"; }

.fa-bitbucket::before { content: "=EF=85=B1"; }

.fa-bitbucket-square::before { content: "=EF=85=B2"; }

.fa-tumblr::before { content: "=EF=85=B3"; }

.fa-tumblr-square::before { content: "=EF=85=B4"; }

.fa-long-arrow-down::before { content: "=EF=85=B5"; }

.fa-long-arrow-up::before { content: "=EF=85=B6"; }

.fa-long-arrow-left::before { content: "=EF=85=B7"; }

.fa-long-arrow-right::before { content: "=EF=85=B8"; }

.fa-apple::before { content: "=EF=85=B9"; }

.fa-windows::before { content: "=EF=85=BA"; }

.fa-android::before { content: "=EF=85=BB"; }

.fa-linux::before { content: "=EF=85=BC"; }

.fa-dribbble::before { content: "=EF=85=BD"; }

.fa-skype::before { content: "=EF=85=BE"; }

.fa-foursquare::before { content: "=EF=86=80"; }

.fa-trello::before { content: "=EF=86=81"; }

.fa-female::before { content: "=EF=86=82"; }

.fa-male::before { content: "=EF=86=83"; }

.fa-gittip::before, .fa-gratipay::before { content: "=EF=86=84"; }

.fa-sun-o::before { content: "=EF=86=85"; }

.fa-moon-o::before { content: "=EF=86=86"; }

.fa-archive::before { content: "=EF=86=87"; }

.fa-bug::before { content: "=EF=86=88"; }

.fa-vk::before { content: "=EF=86=89"; }

.fa-weibo::before { content: "=EF=86=8A"; }

.fa-renren::before { content: "=EF=86=8B"; }

.fa-pagelines::before { content: "=EF=86=8C"; }

.fa-stack-exchange::before { content: "=EF=86=8D"; }

.fa-arrow-circle-o-right::before { content: "=EF=86=8E"; }

.fa-arrow-circle-o-left::before { content: "=EF=86=90"; }

.fa-toggle-left::before, .fa-caret-square-o-left::before { content: "=EF=86=
=91"; }

.fa-dot-circle-o::before { content: "=EF=86=92"; }

.fa-wheelchair::before { content: "=EF=86=93"; }

.fa-vimeo-square::before { content: "=EF=86=94"; }

.fa-turkish-lira::before, .fa-try::before { content: "=EF=86=95"; }

.fa-plus-square-o::before { content: "=EF=86=96"; }

.fa-space-shuttle::before { content: "=EF=86=97"; }

.fa-slack::before { content: "=EF=86=98"; }

.fa-envelope-square::before { content: "=EF=86=99"; }

.fa-wordpress::before { content: "=EF=86=9A"; }

.fa-openid::before { content: "=EF=86=9B"; }

.fa-institution::before, .fa-bank::before, .fa-university::before { content=
: "=EF=86=9C"; }

.fa-mortar-board::before, .fa-graduation-cap::before { content: "=EF=86=9D"=
; }

.fa-yahoo::before { content: "=EF=86=9E"; }

.fa-google::before { content: "=EF=86=A0"; }

.fa-reddit::before { content: "=EF=86=A1"; }

.fa-reddit-square::before { content: "=EF=86=A2"; }

.fa-stumbleupon-circle::before { content: "=EF=86=A3"; }

.fa-stumbleupon::before { content: "=EF=86=A4"; }

.fa-delicious::before { content: "=EF=86=A5"; }

.fa-digg::before { content: "=EF=86=A6"; }

.fa-pied-piper-pp::before { content: "=EF=86=A7"; }

.fa-pied-piper-alt::before { content: "=EF=86=A8"; }

.fa-drupal::before { content: "=EF=86=A9"; }

.fa-joomla::before { content: "=EF=86=AA"; }

.fa-language::before { content: "=EF=86=AB"; }

.fa-fax::before { content: "=EF=86=AC"; }

.fa-building::before { content: "=EF=86=AD"; }

.fa-child::before { content: "=EF=86=AE"; }

.fa-paw::before { content: "=EF=86=B0"; }

.fa-spoon::before { content: "=EF=86=B1"; }

.fa-cube::before { content: "=EF=86=B2"; }

.fa-cubes::before { content: "=EF=86=B3"; }

.fa-behance::before { content: "=EF=86=B4"; }

.fa-behance-square::before { content: "=EF=86=B5"; }

.fa-steam::before { content: "=EF=86=B6"; }

.fa-steam-square::before { content: "=EF=86=B7"; }

.fa-recycle::before { content: "=EF=86=B8"; }

.fa-automobile::before, .fa-car::before { content: "=EF=86=B9"; }

.fa-cab::before, .fa-taxi::before { content: "=EF=86=BA"; }

.fa-tree::before { content: "=EF=86=BB"; }

.fa-spotify::before { content: "=EF=86=BC"; }

.fa-deviantart::before { content: "=EF=86=BD"; }

.fa-soundcloud::before { content: "=EF=86=BE"; }

.fa-database::before { content: "=EF=87=80"; }

.fa-file-pdf-o::before { content: "=EF=87=81"; }

.fa-file-word-o::before { content: "=EF=87=82"; }

.fa-file-excel-o::before { content: "=EF=87=83"; }

.fa-file-powerpoint-o::before { content: "=EF=87=84"; }

.fa-file-photo-o::before, .fa-file-picture-o::before, .fa-file-image-o::bef=
ore { content: "=EF=87=85"; }

.fa-file-zip-o::before, .fa-file-archive-o::before { content: "=EF=87=86"; =
}

.fa-file-sound-o::before, .fa-file-audio-o::before { content: "=EF=87=87"; =
}

.fa-file-movie-o::before, .fa-file-video-o::before { content: "=EF=87=88"; =
}

.fa-file-code-o::before { content: "=EF=87=89"; }

.fa-vine::before { content: "=EF=87=8A"; }

.fa-codepen::before { content: "=EF=87=8B"; }

.fa-jsfiddle::before { content: "=EF=87=8C"; }

.fa-life-bouy::before, .fa-life-buoy::before, .fa-life-saver::before, .fa-s=
upport::before, .fa-life-ring::before { content: "=EF=87=8D"; }

.fa-circle-o-notch::before { content: "=EF=87=8E"; }

.fa-ra::before, .fa-resistance::before, .fa-rebel::before { content: "=EF=
=87=90"; }

.fa-ge::before, .fa-empire::before { content: "=EF=87=91"; }

.fa-git-square::before { content: "=EF=87=92"; }

.fa-git::before { content: "=EF=87=93"; }

.fa-y-combinator-square::before, .fa-yc-square::before, .fa-hacker-news::be=
fore { content: "=EF=87=94"; }

.fa-tencent-weibo::before { content: "=EF=87=95"; }

.fa-qq::before { content: "=EF=87=96"; }

.fa-wechat::before, .fa-weixin::before { content: "=EF=87=97"; }

.fa-send::before, .fa-paper-plane::before { content: "=EF=87=98"; }

.fa-send-o::before, .fa-paper-plane-o::before { content: "=EF=87=99"; }

.fa-history::before { content: "=EF=87=9A"; }

.fa-circle-thin::before { content: "=EF=87=9B"; }

.fa-header::before { content: "=EF=87=9C"; }

.fa-paragraph::before { content: "=EF=87=9D"; }

.fa-sliders::before { content: "=EF=87=9E"; }

.fa-share-alt::before { content: "=EF=87=A0"; }

.fa-share-alt-square::before { content: "=EF=87=A1"; }

.fa-bomb::before { content: "=EF=87=A2"; }

.fa-soccer-ball-o::before, .fa-futbol-o::before { content: "=EF=87=A3"; }

.fa-tty::before { content: "=EF=87=A4"; }

.fa-binoculars::before { content: "=EF=87=A5"; }

.fa-plug::before { content: "=EF=87=A6"; }

.fa-slideshare::before { content: "=EF=87=A7"; }

.fa-twitch::before { content: "=EF=87=A8"; }

.fa-yelp::before { content: "=EF=87=A9"; }

.fa-newspaper-o::before { content: "=EF=87=AA"; }

.fa-wifi::before { content: "=EF=87=AB"; }

.fa-calculator::before { content: "=EF=87=AC"; }

.fa-paypal::before { content: "=EF=87=AD"; }

.fa-google-wallet::before { content: "=EF=87=AE"; }

.fa-cc-visa::before { content: "=EF=87=B0"; }

.fa-cc-mastercard::before { content: "=EF=87=B1"; }

.fa-cc-discover::before { content: "=EF=87=B2"; }

.fa-cc-amex::before { content: "=EF=87=B3"; }

.fa-cc-paypal::before { content: "=EF=87=B4"; }

.fa-cc-stripe::before { content: "=EF=87=B5"; }

.fa-bell-slash::before { content: "=EF=87=B6"; }

.fa-bell-slash-o::before { content: "=EF=87=B7"; }

.fa-trash::before { content: "=EF=87=B8"; }

.fa-copyright::before { content: "=EF=87=B9"; }

.fa-at::before { content: "=EF=87=BA"; }

.fa-eyedropper::before { content: "=EF=87=BB"; }

.fa-paint-brush::before { content: "=EF=87=BC"; }

.fa-birthday-cake::before { content: "=EF=87=BD"; }

.fa-area-chart::before { content: "=EF=87=BE"; }

.fa-pie-chart::before { content: "=EF=88=80"; }

.fa-line-chart::before { content: "=EF=88=81"; }

.fa-lastfm::before { content: "=EF=88=82"; }

.fa-lastfm-square::before { content: "=EF=88=83"; }

.fa-toggle-off::before { content: "=EF=88=84"; }

.fa-toggle-on::before { content: "=EF=88=85"; }

.fa-bicycle::before { content: "=EF=88=86"; }

.fa-bus::before { content: "=EF=88=87"; }

.fa-ioxhost::before { content: "=EF=88=88"; }

.fa-angellist::before { content: "=EF=88=89"; }

.fa-cc::before { content: "=EF=88=8A"; }

.fa-shekel::before, .fa-sheqel::before, .fa-ils::before { content: "=EF=88=
=8B"; }

.fa-meanpath::before { content: "=EF=88=8C"; }

.fa-buysellads::before { content: "=EF=88=8D"; }

.fa-connectdevelop::before { content: "=EF=88=8E"; }

.fa-dashcube::before { content: "=EF=88=90"; }

.fa-forumbee::before { content: "=EF=88=91"; }

.fa-leanpub::before { content: "=EF=88=92"; }

.fa-sellsy::before { content: "=EF=88=93"; }

.fa-shirtsinbulk::before { content: "=EF=88=94"; }

.fa-simplybuilt::before { content: "=EF=88=95"; }

.fa-skyatlas::before { content: "=EF=88=96"; }

.fa-cart-plus::before { content: "=EF=88=97"; }

.fa-cart-arrow-down::before { content: "=EF=88=98"; }

.fa-diamond::before { content: "=EF=88=99"; }

.fa-ship::before { content: "=EF=88=9A"; }

.fa-user-secret::before { content: "=EF=88=9B"; }

.fa-motorcycle::before { content: "=EF=88=9C"; }

.fa-street-view::before { content: "=EF=88=9D"; }

.fa-heartbeat::before { content: "=EF=88=9E"; }

.fa-venus::before { content: "=EF=88=A1"; }

.fa-mars::before { content: "=EF=88=A2"; }

.fa-mercury::before { content: "=EF=88=A3"; }

.fa-intersex::before, .fa-transgender::before { content: "=EF=88=A4"; }

.fa-transgender-alt::before { content: "=EF=88=A5"; }

.fa-venus-double::before { content: "=EF=88=A6"; }

.fa-mars-double::before { content: "=EF=88=A7"; }

.fa-venus-mars::before { content: "=EF=88=A8"; }

.fa-mars-stroke::before { content: "=EF=88=A9"; }

.fa-mars-stroke-v::before { content: "=EF=88=AA"; }

.fa-mars-stroke-h::before { content: "=EF=88=AB"; }

.fa-neuter::before { content: "=EF=88=AC"; }

.fa-genderless::before { content: "=EF=88=AD"; }

.fa-facebook-official::before { content: "=EF=88=B0"; }

.fa-pinterest-p::before { content: "=EF=88=B1"; }

.fa-whatsapp::before { content: "=EF=88=B2"; }

.fa-server::before { content: "=EF=88=B3"; }

.fa-user-plus::before { content: "=EF=88=B4"; }

.fa-user-times::before { content: "=EF=88=B5"; }

.fa-hotel::before, .fa-bed::before { content: "=EF=88=B6"; }

.fa-viacoin::before { content: "=EF=88=B7"; }

.fa-train::before { content: "=EF=88=B8"; }

.fa-subway::before { content: "=EF=88=B9"; }

.fa-medium::before { content: "=EF=88=BA"; }

.fa-yc::before, .fa-y-combinator::before { content: "=EF=88=BB"; }

.fa-optin-monster::before { content: "=EF=88=BC"; }

.fa-opencart::before { content: "=EF=88=BD"; }

.fa-expeditedssl::before { content: "=EF=88=BE"; }

.fa-battery-4::before, .fa-battery::before, .fa-battery-full::before { cont=
ent: "=EF=89=80"; }

.fa-battery-3::before, .fa-battery-three-quarters::before { content: "=EF=
=89=81"; }

.fa-battery-2::before, .fa-battery-half::before { content: "=EF=89=82"; }

.fa-battery-1::before, .fa-battery-quarter::before { content: "=EF=89=83"; =
}

.fa-battery-0::before, .fa-battery-empty::before { content: "=EF=89=84"; }

.fa-mouse-pointer::before { content: "=EF=89=85"; }

.fa-i-cursor::before { content: "=EF=89=86"; }

.fa-object-group::before { content: "=EF=89=87"; }

.fa-object-ungroup::before { content: "=EF=89=88"; }

.fa-sticky-note::before { content: "=EF=89=89"; }

.fa-sticky-note-o::before { content: "=EF=89=8A"; }

.fa-cc-jcb::before { content: "=EF=89=8B"; }

.fa-cc-diners-club::before { content: "=EF=89=8C"; }

.fa-clone::before { content: "=EF=89=8D"; }

.fa-balance-scale::before { content: "=EF=89=8E"; }

.fa-hourglass-o::before { content: "=EF=89=90"; }

.fa-hourglass-1::before, .fa-hourglass-start::before { content: "=EF=89=91"=
; }

.fa-hourglass-2::before, .fa-hourglass-half::before { content: "=EF=89=92";=
 }

.fa-hourglass-3::before, .fa-hourglass-end::before { content: "=EF=89=93"; =
}

.fa-hourglass::before { content: "=EF=89=94"; }

.fa-hand-grab-o::before, .fa-hand-rock-o::before { content: "=EF=89=95"; }

.fa-hand-stop-o::before, .fa-hand-paper-o::before { content: "=EF=89=96"; }

.fa-hand-scissors-o::before { content: "=EF=89=97"; }

.fa-hand-lizard-o::before { content: "=EF=89=98"; }

.fa-hand-spock-o::before { content: "=EF=89=99"; }

.fa-hand-pointer-o::before { content: "=EF=89=9A"; }

.fa-hand-peace-o::before { content: "=EF=89=9B"; }

.fa-trademark::before { content: "=EF=89=9C"; }

.fa-registered::before { content: "=EF=89=9D"; }

.fa-creative-commons::before { content: "=EF=89=9E"; }

.fa-gg::before { content: "=EF=89=A0"; }

.fa-gg-circle::before { content: "=EF=89=A1"; }

.fa-tripadvisor::before { content: "=EF=89=A2"; }

.fa-odnoklassniki::before { content: "=EF=89=A3"; }

.fa-odnoklassniki-square::before { content: "=EF=89=A4"; }

.fa-get-pocket::before { content: "=EF=89=A5"; }

.fa-wikipedia-w::before { content: "=EF=89=A6"; }

.fa-safari::before { content: "=EF=89=A7"; }

.fa-chrome::before { content: "=EF=89=A8"; }

.fa-firefox::before { content: "=EF=89=A9"; }

.fa-opera::before { content: "=EF=89=AA"; }

.fa-internet-explorer::before { content: "=EF=89=AB"; }

.fa-tv::before, .fa-television::before { content: "=EF=89=AC"; }

.fa-contao::before { content: "=EF=89=AD"; }

.fa-500px::before { content: "=EF=89=AE"; }

.fa-amazon::before { content: "=EF=89=B0"; }

.fa-calendar-plus-o::before { content: "=EF=89=B1"; }

.fa-calendar-minus-o::before { content: "=EF=89=B2"; }

.fa-calendar-times-o::before { content: "=EF=89=B3"; }

.fa-calendar-check-o::before { content: "=EF=89=B4"; }

.fa-industry::before { content: "=EF=89=B5"; }

.fa-map-pin::before { content: "=EF=89=B6"; }

.fa-map-signs::before { content: "=EF=89=B7"; }

.fa-map-o::before { content: "=EF=89=B8"; }

.fa-map::before { content: "=EF=89=B9"; }

.fa-commenting::before { content: "=EF=89=BA"; }

.fa-commenting-o::before { content: "=EF=89=BB"; }

.fa-houzz::before { content: "=EF=89=BC"; }

.fa-vimeo::before { content: "=EF=89=BD"; }

.fa-black-tie::before { content: "=EF=89=BE"; }

.fa-fonticons::before { content: "=EF=8A=80"; }

.fa-reddit-alien::before { content: "=EF=8A=81"; }

.fa-edge::before { content: "=EF=8A=82"; }

.fa-credit-card-alt::before { content: "=EF=8A=83"; }

.fa-codiepie::before { content: "=EF=8A=84"; }

.fa-modx::before { content: "=EF=8A=85"; }

.fa-fort-awesome::before { content: "=EF=8A=86"; }

.fa-usb::before { content: "=EF=8A=87"; }

.fa-product-hunt::before { content: "=EF=8A=88"; }

.fa-mixcloud::before { content: "=EF=8A=89"; }

.fa-scribd::before { content: "=EF=8A=8A"; }

.fa-pause-circle::before { content: "=EF=8A=8B"; }

.fa-pause-circle-o::before { content: "=EF=8A=8C"; }

.fa-stop-circle::before { content: "=EF=8A=8D"; }

.fa-stop-circle-o::before { content: "=EF=8A=8E"; }

.fa-shopping-bag::before { content: "=EF=8A=90"; }

.fa-shopping-basket::before { content: "=EF=8A=91"; }

.fa-hashtag::before { content: "=EF=8A=92"; }

.fa-bluetooth::before { content: "=EF=8A=93"; }

.fa-bluetooth-b::before { content: "=EF=8A=94"; }

.fa-percent::before { content: "=EF=8A=95"; }

.fa-gitlab::before { content: "=EF=8A=96"; }

.fa-wpbeginner::before { content: "=EF=8A=97"; }

.fa-wpforms::before { content: "=EF=8A=98"; }

.fa-envira::before { content: "=EF=8A=99"; }

.fa-universal-access::before { content: "=EF=8A=9A"; }

.fa-wheelchair-alt::before { content: "=EF=8A=9B"; }

.fa-question-circle-o::before { content: "=EF=8A=9C"; }

.fa-blind::before { content: "=EF=8A=9D"; }

.fa-audio-description::before { content: "=EF=8A=9E"; }

.fa-volume-control-phone::before { content: "=EF=8A=A0"; }

.fa-braille::before { content: "=EF=8A=A1"; }

.fa-assistive-listening-systems::before { content: "=EF=8A=A2"; }

.fa-asl-interpreting::before, .fa-american-sign-language-interpreting::befo=
re { content: "=EF=8A=A3"; }

.fa-deafness::before, .fa-hard-of-hearing::before, .fa-deaf::before { conte=
nt: "=EF=8A=A4"; }

.fa-glide::before { content: "=EF=8A=A5"; }

.fa-glide-g::before { content: "=EF=8A=A6"; }

.fa-signing::before, .fa-sign-language::before { content: "=EF=8A=A7"; }

.fa-low-vision::before { content: "=EF=8A=A8"; }

.fa-viadeo::before { content: "=EF=8A=A9"; }

.fa-viadeo-square::before { content: "=EF=8A=AA"; }

.fa-snapchat::before { content: "=EF=8A=AB"; }

.fa-snapchat-ghost::before { content: "=EF=8A=AC"; }

.fa-snapchat-square::before { content: "=EF=8A=AD"; }

.fa-pied-piper::before { content: "=EF=8A=AE"; }

.fa-first-order::before { content: "=EF=8A=B0"; }

.fa-yoast::before { content: "=EF=8A=B1"; }

.fa-themeisle::before { content: "=EF=8A=B2"; }

.fa-google-plus-circle::before, .fa-google-plus-official::before { content:=
 "=EF=8A=B3"; }

.fa-fa::before, .fa-font-awesome::before { content: "=EF=8A=B4"; }

.fa-handshake-o::before { content: "=EF=8A=B5"; }

.fa-envelope-open::before { content: "=EF=8A=B6"; }

.fa-envelope-open-o::before { content: "=EF=8A=B7"; }

.fa-linode::before { content: "=EF=8A=B8"; }

.fa-address-book::before { content: "=EF=8A=B9"; }

.fa-address-book-o::before { content: "=EF=8A=BA"; }

.fa-vcard::before, .fa-address-card::before { content: "=EF=8A=BB"; }

.fa-vcard-o::before, .fa-address-card-o::before { content: "=EF=8A=BC"; }

.fa-user-circle::before { content: "=EF=8A=BD"; }

.fa-user-circle-o::before { content: "=EF=8A=BE"; }

.fa-user-o::before { content: "=EF=8B=80"; }

.fa-id-badge::before { content: "=EF=8B=81"; }

.fa-drivers-license::before, .fa-id-card::before { content: "=EF=8B=82"; }

.fa-drivers-license-o::before, .fa-id-card-o::before { content: "=EF=8B=83"=
; }

.fa-quora::before { content: "=EF=8B=84"; }

.fa-free-code-camp::before { content: "=EF=8B=85"; }

.fa-telegram::before { content: "=EF=8B=86"; }

.fa-thermometer-4::before, .fa-thermometer::before, .fa-thermometer-full::b=
efore { content: "=EF=8B=87"; }

.fa-thermometer-3::before, .fa-thermometer-three-quarters::before { content=
: "=EF=8B=88"; }

.fa-thermometer-2::before, .fa-thermometer-half::before { content: "=EF=8B=
=89"; }

.fa-thermometer-1::before, .fa-thermometer-quarter::before { content: "=EF=
=8B=8A"; }

.fa-thermometer-0::before, .fa-thermometer-empty::before { content: "=EF=8B=
=8B"; }

.fa-shower::before { content: "=EF=8B=8C"; }

.fa-bathtub::before, .fa-s15::before, .fa-bath::before { content: "=EF=8B=
=8D"; }

.fa-podcast::before { content: "=EF=8B=8E"; }

.fa-window-maximize::before { content: "=EF=8B=90"; }

.fa-window-minimize::before { content: "=EF=8B=91"; }

.fa-window-restore::before { content: "=EF=8B=92"; }

.fa-times-rectangle::before, .fa-window-close::before { content: "=EF=8B=93=
"; }

.fa-times-rectangle-o::before, .fa-window-close-o::before { content: "=EF=
=8B=94"; }

.fa-bandcamp::before { content: "=EF=8B=95"; }

.fa-grav::before { content: "=EF=8B=96"; }

.fa-etsy::before { content: "=EF=8B=97"; }

.fa-imdb::before { content: "=EF=8B=98"; }

.fa-ravelry::before { content: "=EF=8B=99"; }

.fa-eercast::before { content: "=EF=8B=9A"; }

.fa-microchip::before { content: "=EF=8B=9B"; }

.fa-snowflake-o::before { content: "=EF=8B=9C"; }

.fa-superpowers::before { content: "=EF=8B=9D"; }

.fa-wpexplorer::before { content: "=EF=8B=9E"; }

.fa-meetup::before { content: "=EF=8B=A0"; }

.sr-only { position: absolute; width: 1px; height: 1px; padding: 0px; margi=
n: -1px; overflow: hidden; clip: rect(0px, 0px, 0px, 0px); border: 0px; }

.sr-only-focusable:active, .sr-only-focusable:focus { position: static; wid=
th: auto; height: auto; margin: 0px; overflow: visible; clip: auto; }

.sr-only-focusable:active, .sr-only-focusable:focus { position: static; wid=
th: auto; height: auto; margin: 0px; overflow: visible; clip: auto; }

.modal.fade .modal-dialog { transform: translate(0px, 0px); }

code { color: rgb(0, 0, 0); }

pre { font-size: inherit; line-height: inherit; }

label { font-weight: normal; }

.border-box-sizing { box-sizing: border-box; }

.corner-all { border-radius: 2px; }

.no-padding { padding: 0px; }

.hbox { -webkit-box-orient: horizontal; -webkit-box-align: stretch; display=
: flex; flex-direction: row; align-items: stretch; }

.hbox > * { -webkit-box-flex: 0; flex: 0 0 auto; }

.vbox { -webkit-box-orient: vertical; -webkit-box-align: stretch; display: =
flex; flex-direction: column; align-items: stretch; }

.vbox > * { -webkit-box-flex: 0; flex: 0 0 auto; }

.hbox.reverse, .vbox.reverse, .reverse { -webkit-box-direction: reverse; fl=
ex-direction: row-reverse; }

.hbox.box-flex0, .vbox.box-flex0, .box-flex0 { -webkit-box-flex: 0; flex: 0=
 0 auto; width: auto; }

.hbox.box-flex1, .vbox.box-flex1, .box-flex1 { -webkit-box-flex: 1; flex: 1=
 1 0%; }

.hbox.box-flex, .vbox.box-flex, .box-flex { -webkit-box-flex: 1; flex: 1 1 =
0%; }

.hbox.box-flex2, .vbox.box-flex2, .box-flex2 { -webkit-box-flex: 2; flex: 2=
 1 0%; }

.box-group1 { }

.box-group2 { }

.hbox.start, .vbox.start, .start { -webkit-box-pack: start; justify-content=
: flex-start; }

.hbox.end, .vbox.end, .end { -webkit-box-pack: end; justify-content: flex-e=
nd; }

.hbox.center, .vbox.center, .center { -webkit-box-pack: center; justify-con=
tent: center; }

.hbox.baseline, .vbox.baseline, .baseline { }

.hbox.stretch, .vbox.stretch, .stretch { justify-content: stretch; }

.hbox.align-start, .vbox.align-start, .align-start { -webkit-box-align: sta=
rt; align-items: flex-start; }

.hbox.align-end, .vbox.align-end, .align-end { -webkit-box-align: end; alig=
n-items: flex-end; }

.hbox.align-center, .vbox.align-center, .align-center { -webkit-box-align: =
center; align-items: center; }

.hbox.align-baseline, .vbox.align-baseline, .align-baseline { -webkit-box-a=
lign: baseline; align-items: baseline; }

.hbox.align-stretch, .vbox.align-stretch, .align-stretch { -webkit-box-alig=
n: stretch; align-items: stretch; }

div.error { margin: 2em; text-align: center; }

div.error > h1 { font-size: 500%; line-height: normal; }

div.error > p { font-size: 200%; line-height: normal; }

div.traceback-wrapper { text-align: left; max-width: 800px; margin: auto; }

div.traceback-wrapper pre.traceback { max-height: 600px; overflow: auto; }

body { background-color: rgb(255, 255, 255); position: absolute; inset: 0px=
; overflow: visible; }

body > #header { display: none; background-color: rgb(255, 255, 255); posit=
ion: relative; z-index: 100; }

body > #header #header-container { display: flex; flex-direction: row; just=
ify-content: space-between; padding: 5px; box-sizing: border-box; }

body > #header .header-bar { width: 100%; height: 1px; background: rgb(231,=
 231, 231); margin-bottom: -1px; }

@media print {
  body > #header { display: none !important; }
}

#header-spacer { width: 100%; visibility: hidden; }

@media print {
  #header-spacer { display: none; }
}

#ipython_notebook { padding-left: 0px; padding-top: 1px; padding-bottom: 1p=
x; }

[dir=3D"rtl"] #ipython_notebook { margin-right: 10px; margin-left: 0px; }

[dir=3D"rtl"] #ipython_notebook.pull-left { float: right !important; }

.flex-spacer { flex: 1 1 0%; }

#noscript { width: auto; padding-top: 16px; padding-bottom: 16px; text-alig=
n: center; font-size: 22px; color: red; font-weight: bold; }

#ipython_notebook img { height: 28px; }

#site { width: 100%; display: none; box-sizing: border-box; overflow: auto;=
 }

@media print {
  #site { height: auto !important; }
}

.ui-button .ui-button-text { padding: 0.2em 0.8em; font-size: 77%; }

input.ui-button { padding: 0.3em 0.9em; }

span#kernel_logo_widget { margin: 0px 10px; }

span#login_widget { float: right; }

[dir=3D"rtl"] span#login_widget { float: left; }

span#login_widget > .button, #logout, #shutdown { color: rgb(51, 51, 51); b=
ackground-color: rgb(255, 255, 255); border-color: rgb(204, 204, 204); marg=
in-left: 10px; }

span#login_widget > .button:focus, #logout:focus, #shutdown:focus, span#log=
in_widget > .button.focus, #logout.focus, #shutdown.focus { color: rgb(51, =
51, 51); background-color: rgb(230, 230, 230); border-color: rgb(140, 140, =
140); }

span#login_widget > .button:hover, #logout:hover, #shutdown:hover { color: =
rgb(51, 51, 51); background-color: rgb(230, 230, 230); border-color: rgb(17=
3, 173, 173); }

span#login_widget > .button:active, #logout:active, #shutdown:active, span#=
login_widget > .button.active, #logout.active, #shutdown.active, .open > .d=
ropdown-togglespan#login_widget > .button, .open > .dropdown-toggle#logout,=
 .open > .dropdown-toggle#shutdown { color: rgb(51, 51, 51); background-col=
or: rgb(230, 230, 230); background-image: none; border-color: rgb(173, 173,=
 173); }

span#login_widget > .button:active:hover, #logout:active:hover, #shutdown:a=
ctive:hover, span#login_widget > .button.active:hover, #logout.active:hover=
, #shutdown.active:hover, .open > .dropdown-togglespan#login_widget > .butt=
on:hover, .open > .dropdown-toggle#logout:hover, .open > .dropdown-toggle#s=
hutdown:hover, span#login_widget > .button:active:focus, #logout:active:foc=
us, #shutdown:active:focus, span#login_widget > .button.active:focus, #logo=
ut.active:focus, #shutdown.active:focus, .open > .dropdown-togglespan#login=
_widget > .button:focus, .open > .dropdown-toggle#logout:focus, .open > .dr=
opdown-toggle#shutdown:focus, span#login_widget > .button:active.focus, #lo=
gout:active.focus, #shutdown:active.focus, span#login_widget > .button.acti=
ve.focus, #logout.active.focus, #shutdown.active.focus, .open > .dropdown-t=
ogglespan#login_widget > .button.focus, .open > .dropdown-toggle#logout.foc=
us, .open > .dropdown-toggle#shutdown.focus { color: rgb(51, 51, 51); backg=
round-color: rgb(212, 212, 212); border-color: rgb(140, 140, 140); }

span#login_widget > .button.disabled:hover, #logout.disabled:hover, #shutdo=
wn.disabled:hover, span#login_widget > .button[disabled]:hover, #logout[dis=
abled]:hover, #shutdown[disabled]:hover, fieldset[disabled] span#login_widg=
et > .button:hover, fieldset[disabled] #logout:hover, fieldset[disabled] #s=
hutdown:hover, span#login_widget > .button.disabled:focus, #logout.disabled=
:focus, #shutdown.disabled:focus, span#login_widget > .button[disabled]:foc=
us, #logout[disabled]:focus, #shutdown[disabled]:focus, fieldset[disabled] =
span#login_widget > .button:focus, fieldset[disabled] #logout:focus, fields=
et[disabled] #shutdown:focus, span#login_widget > .button.disabled.focus, #=
logout.disabled.focus, #shutdown.disabled.focus, span#login_widget > .butto=
n[disabled].focus, #logout[disabled].focus, #shutdown[disabled].focus, fiel=
dset[disabled] span#login_widget > .button.focus, fieldset[disabled] #logou=
t.focus, fieldset[disabled] #shutdown.focus { background-color: rgb(255, 25=
5, 255); border-color: rgb(204, 204, 204); }

span#login_widget > .button .badge, #logout .badge, #shutdown .badge { colo=
r: rgb(255, 255, 255); background-color: rgb(51, 51, 51); }

.nav-header { text-transform: none; }

#header > span { margin-top: 10px; }

.modal_stretch .modal-dialog { -webkit-box-orient: vertical; -webkit-box-al=
ign: stretch; display: flex; flex-direction: column; align-items: stretch; =
min-height: 80vh; }

.modal_stretch .modal-dialog .modal-body { max-height: calc(-200px + 100vh)=
; overflow: auto; flex: 1 1 0%; }

.modal-header { cursor: move; }

@media (min-width: 768px) {
  .modal .modal-dialog { width: 700px; }
}

@media (min-width: 768px) {
  select.form-control { margin-left: 12px; margin-right: 12px; }
}

[dir=3D"rtl"] .modal-footer { text-align: left !important; }

[dir=3D"rtl"] .close { float: left; }

[dir=3D"rtl"] .fa-step-forward::before { content: "=EF=81=88"; }

.center-nav { display: inline-block; margin-bottom: -4px; }

[dir=3D"rtl"] .center-nav form.pull-left { float: right !important; }

[dir=3D"rtl"] .center-nav .navbar-text { float: right; }

[dir=3D"rtl"] .navbar-inner { text-align: right; }

[dir=3D"rtl"] div.text-left { text-align: right; }

.alternate_upload { display: inline; }

.alternate_upload.form { padding: 0px; margin: 0px; }

.alternate_upload input.fileinput { position: absolute; display: block; wid=
th: 100%; height: 100%; overflow: hidden; cursor: pointer; opacity: 0; z-in=
dex: 2; }

.alternate_upload .btn-xs > input.fileinput { margin: -1px -5px; }

.alternate_upload .btn-upload { position: relative; height: 22px; }

::-webkit-file-upload-button { cursor: pointer; }

ul#tabs { margin-bottom: 4px; }

ul#tabs a { padding-top: 6px; padding-bottom: 4px; }

[dir=3D"rtl"] ul#tabs.nav-tabs > li { float: right; }

[dir=3D"rtl"] ul#tabs.nav.nav-tabs { padding-right: 0px; }

ul.breadcrumb a:focus, ul.breadcrumb a:hover { text-decoration: none; }

ul.breadcrumb i.icon-home { font-size: 16px; margin-right: 4px; }

ul.breadcrumb span { color: rgb(94, 94, 94); }

.list_toolbar { padding: 4px 0px; vertical-align: middle; }

.list_toolbar .tree-buttons { padding-top: 1px; }

[dir=3D"rtl"] .list_toolbar .tree-buttons .pull-right { float: left !import=
ant; }

[dir=3D"rtl"] .list_toolbar .col-sm-4, [dir=3D"rtl"] .list_toolbar .col-sm-=
8 { float: right; }

.dynamic-buttons { padding-top: 3px; display: inline-block; width: 400px; }

.list_toolbar [class*=3D"span"] { min-height: 24px; }

.list_header { font-weight: bold; background-color: rgb(238, 238, 238); }

.list_placeholder { font-weight: bold; padding: 4px 7px; }

.list_container { margin-top: 4px; margin-bottom: 20px; border: 1px solid r=
gb(221, 221, 221); border-radius: 2px; }

.list_container > div { border-bottom: 1px solid rgb(221, 221, 221); }

.list_container > div:hover .list-item { background-color: red; }

.list_container > div:last-child { border: none; }

.list_item:hover .list_item { background-color: rgb(221, 221, 221); }

.list_item a { text-decoration: none; }

.list_item:hover { background-color: rgb(250, 250, 250); }

.list_header > div, .list_item > div { padding: 4px 7px; line-height: 22px;=
 }

.list_header > div input, .list_item > div input { margin-right: 7px; margi=
n-left: 14px; vertical-align: text-bottom; line-height: 22px; position: rel=
ative; top: -1px; }

.list_header > div .item_link, .list_item > div .item_link { margin-left: -=
1px; vertical-align: baseline; line-height: 22px; }

[dir=3D"rtl"] .list_item > div input { margin-right: 0px; }

.new-file input[type=3D"checkbox"] { visibility: hidden; }

.item_name { line-height: 22px; height: 24px; }

.item_icon { font-size: 14px; color: rgb(94, 94, 94); margin-right: 7px; ma=
rgin-left: 7px; line-height: 22px; vertical-align: baseline; }

.item_modified { margin-right: 7px; margin-left: 7px; }

.file_size { width: 65px; text-align: right; }

[dir=3D"rtl"] .item_modified.pull-right { float: left !important; }

.item_buttons { line-height: 1em; margin-left: -5px; }

.item_buttons .btn, .item_buttons .btn-group, .item_buttons .input-group { =
float: left; }

.item_buttons > .btn, .item_buttons > .btn-group, .item_buttons > .input-gr=
oup { margin-left: 5px; }

.item_buttons .btn { min-width: 13ex; }

.item_buttons .running-indicator { padding-top: 4px; color: rgb(45, 103, 45=
); }

.item_buttons .kernel-name { padding-top: 4px; color: rgb(91, 192, 222); ma=
rgin-right: 7px; float: left; }

[dir=3D"rtl"] .item_buttons.pull-right { float: left !important; }

[dir=3D"rtl"] .item_buttons .kernel-name { margin-left: 7px; float: right; =
color: rgb(72, 158, 184); font-weight: 700; }

.toolbar_info { height: 24px; line-height: 24px; }

.list_item input:not([type=3D"checkbox"]) { padding-top: 3px; padding-botto=
m: 3px; height: 22px; line-height: 14px; margin: 0px; }

.highlight_text { color: blue; }

#project_name { display: inline-block; padding-left: 7px; margin-left: -2px=
; color: rgb(31, 83, 129); }

#project_name > .breadcrumb { padding: 0px; margin-bottom: 0px; background-=
color: transparent; font-weight: bold; }

.sort_button { display: inline-block; padding-left: 7px; }

[dir=3D"rtl"] .sort_button.pull-right { float: left !important; }

#tree-selector { padding-right: 0px; }

#button-select-all { min-width: 50px; }

[dir=3D"rtl"] #button-select-all.btn { float: right; }

#select-all { margin-left: 7px; margin-right: 2px; margin-top: 2px; height:=
 16px; }

[dir=3D"rtl"] #select-all.pull-left { float: right !important; }

.menu_icon { margin-right: 2px; }

.tab-content .row { margin-left: 0px; margin-right: 0px; }

.folder_icon::before { display: inline-block; font-style: normal; font-vari=
ant: normal; font-kerning: auto; font-optical-sizing: auto; font-feature-se=
ttings: normal; font-variation-settings: normal; font-weight: normal; font-=
stretch: normal; line-height: 1; font-family: FontAwesome; font-size: inher=
it; text-rendering: auto; -webkit-font-smoothing: antialiased; content: "=
=EF=84=94"; }

.notebook_icon::before { display: inline-block; font-style: normal; font-va=
riant: normal; font-kerning: auto; font-optical-sizing: auto; font-feature-=
settings: normal; font-variation-settings: normal; font-weight: normal; fon=
t-stretch: normal; line-height: 1; font-family: FontAwesome; font-size: inh=
erit; text-rendering: auto; -webkit-font-smoothing: antialiased; content: "=
=EF=80=AD"; position: relative; top: -1px; }

.running_notebook_icon::before { display: inline-block; font-style: normal;=
 font-variant: normal; font-kerning: auto; font-optical-sizing: auto; font-=
feature-settings: normal; font-variation-settings: normal; font-weight: nor=
mal; font-stretch: normal; line-height: 1; font-family: FontAwesome; font-s=
ize: inherit; text-rendering: auto; -webkit-font-smoothing: antialiased; co=
ntent: "=EF=80=AD"; position: relative; top: -1px; color: rgb(92, 184, 92);=
 }

.file_icon::before { display: inline-block; font-style: normal; font-varian=
t: normal; font-kerning: auto; font-optical-sizing: auto; font-feature-sett=
ings: normal; font-variation-settings: normal; font-weight: normal; font-st=
retch: normal; line-height: 1; font-family: FontAwesome; font-size: inherit=
; text-rendering: auto; -webkit-font-smoothing: antialiased; content: "=EF=
=80=96"; position: relative; top: -2px; }

#notebook_toolbar .pull-right { padding-top: 0px; margin-right: -1px; }

ul#new-menu { left: auto; right: 0px; }

#new-menu .dropdown-header { font-size: 10px; border-bottom: 1px solid rgb(=
229, 229, 229); padding: 0px 0px 3px; margin: -3px 20px 0px; }

.kernel-menu-icon { padding-right: 12px; width: 24px; content: "=EF=82=96";=
 }

.kernel-menu-icon::before { content: "=EF=82=96"; }

.kernel-menu-icon-current::before { content: "=EF=80=8C"; }

#tab_content { padding-top: 20px; }

#running .panel-group .panel { margin-top: 3px; margin-bottom: 1em; }

#running .panel-group .panel .panel-heading { background-color: rgb(238, 23=
8, 238); padding: 4px 7px; line-height: 22px; }

#running .panel-group .panel .panel-heading a:focus, #running .panel-group =
.panel .panel-heading a:hover { text-decoration: none; }

#running .panel-group .panel .panel-body { padding: 0px; }

#running .panel-group .panel .panel-body .list_container { margin-top: 0px;=
 margin-bottom: 0px; border: 0px; border-radius: 0px; }

#running .panel-group .panel .panel-body .list_container .list_item { borde=
r-bottom: 1px solid rgb(221, 221, 221); }

#running .panel-group .panel .panel-body .list_container .list_item:last-ch=
ild { border-bottom: 0px; }

.delete-button { display: none; }

.duplicate-button { display: none; }

.rename-button { display: none; }

.move-button { display: none; }

.download-button { display: none; }

.shutdown-button { display: none; }

.dynamic-instructions { display: inline-block; padding-top: 4px; }

.dynamic-buttons button:focus + [role=3D"tooltip"] { visibility: visible; o=
pacity: 1; }

.dynamic-buttons [role=3D"tooltip"] { position: absolute; top: 70%; display=
: inline; visibility: hidden; background-color: rgb(240, 239, 239); color: =
rgb(8, 8, 8); text-align: center; padding: 3px; outline: grey auto 1px; out=
line-offset: -2px; z-index: 1; opacity: 0; transition: opacity 0.6s ease 0s=
; margin: 3px; font-size: 10px; }

.selected-keymap i.fa { padding: 0px 5px; }

.selected-keymap i.fa::before { content: "=EF=80=8C"; }

#mode-menu { overflow: auto; max-height: 20em; }

.edit_app #header { box-shadow: rgba(87, 87, 87, 0.2) 0px 0px 12px 1px; }

.edit_app #menubar .navbar { margin-bottom: -1px; }

.dirty-indicator { display: inline-block; font-style: normal; font-variant:=
 normal; font-kerning: auto; font-optical-sizing: auto; font-feature-settin=
gs: normal; font-variation-settings: normal; font-weight: normal; font-stre=
tch: normal; line-height: 1; font-family: FontAwesome; font-size: inherit; =
text-rendering: auto; -webkit-font-smoothing: antialiased; width: 20px; }

.dirty-indicator.fa-pull-left { margin-right: 0.3em; }

.dirty-indicator.fa-pull-right { margin-left: 0.3em; }

.dirty-indicator.pull-left { margin-right: 0.3em; }

.dirty-indicator.pull-right { margin-left: 0.3em; }

.dirty-indicator-dirty { display: inline-block; font-style: normal; font-va=
riant: normal; font-kerning: auto; font-optical-sizing: auto; font-feature-=
settings: normal; font-variation-settings: normal; font-weight: normal; fon=
t-stretch: normal; line-height: 1; font-family: FontAwesome; font-size: inh=
erit; text-rendering: auto; -webkit-font-smoothing: antialiased; width: 20p=
x; }

.dirty-indicator-dirty.fa-pull-left { margin-right: 0.3em; }

.dirty-indicator-dirty.fa-pull-right { margin-left: 0.3em; }

.dirty-indicator-dirty.pull-left { margin-right: 0.3em; }

.dirty-indicator-dirty.pull-right { margin-left: 0.3em; }

.dirty-indicator-clean { display: inline-block; font-style: normal; font-va=
riant: normal; font-kerning: auto; font-optical-sizing: auto; font-feature-=
settings: normal; font-variation-settings: normal; font-weight: normal; fon=
t-stretch: normal; line-height: 1; font-family: FontAwesome; font-size: inh=
erit; text-rendering: auto; -webkit-font-smoothing: antialiased; width: 20p=
x; }

.dirty-indicator-clean.fa-pull-left { margin-right: 0.3em; }

.dirty-indicator-clean.fa-pull-right { margin-left: 0.3em; }

.dirty-indicator-clean.pull-left { margin-right: 0.3em; }

.dirty-indicator-clean.pull-right { margin-left: 0.3em; }

.dirty-indicator-clean::before { display: inline-block; font-style: normal;=
 font-variant: normal; font-kerning: auto; font-optical-sizing: auto; font-=
feature-settings: normal; font-variation-settings: normal; font-weight: nor=
mal; font-stretch: normal; line-height: 1; font-family: FontAwesome; font-s=
ize: inherit; text-rendering: auto; -webkit-font-smoothing: antialiased; co=
ntent: "=EF=80=8C"; }

#filename { font-size: 16pt; display: table; padding: 0px 5px; }

#current-mode { padding-left: 5px; padding-right: 5px; }

#texteditor-backdrop { padding-top: 20px; padding-bottom: 20px; }

@media not print {
  #texteditor-backdrop { background-color: rgb(238, 238, 238); }
}

@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter, #textedito=
r-backdrop #texteditor-container .CodeMirror-gutters { background-color: rg=
b(255, 255, 255); }
}

@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter, #textedito=
r-backdrop #texteditor-container .CodeMirror-gutters { background-color: rg=
b(255, 255, 255); }
}

@media not print {
  #texteditor-backdrop #texteditor-container { padding: 0px; background-col=
or: rgb(255, 255, 255); box-shadow: rgba(87, 87, 87, 0.2) 0px 0px 12px 1px;=
 }
}

.CodeMirror-dialog { background-color: rgb(255, 255, 255); }

.ansi-black-fg { color: rgb(62, 66, 77); }

.ansi-black-bg { background-color: rgb(62, 66, 77); }

.ansi-black-intense-fg { color: rgb(40, 44, 54); }

.ansi-black-intense-bg { background-color: rgb(40, 44, 54); }

.ansi-red-fg { color: rgb(231, 92, 88); }

.ansi-red-bg { background-color: rgb(231, 92, 88); }

.ansi-red-intense-fg { color: rgb(178, 43, 49); }

.ansi-red-intense-bg { background-color: rgb(178, 43, 49); }

.ansi-green-fg { color: rgb(0, 162, 80); }

.ansi-green-bg { background-color: rgb(0, 162, 80); }

.ansi-green-intense-fg { color: rgb(0, 116, 39); }

.ansi-green-intense-bg { background-color: rgb(0, 116, 39); }

.ansi-yellow-fg { color: rgb(221, 182, 43); }

.ansi-yellow-bg { background-color: rgb(221, 182, 43); }

.ansi-yellow-intense-fg { color: rgb(178, 125, 18); }

.ansi-yellow-intense-bg { background-color: rgb(178, 125, 18); }

.ansi-blue-fg { color: rgb(32, 143, 251); }

.ansi-blue-bg { background-color: rgb(32, 143, 251); }

.ansi-blue-intense-fg { color: rgb(0, 101, 202); }

.ansi-blue-intense-bg { background-color: rgb(0, 101, 202); }

.ansi-magenta-fg { color: rgb(209, 96, 196); }

.ansi-magenta-bg { background-color: rgb(209, 96, 196); }

.ansi-magenta-intense-fg { color: rgb(160, 49, 150); }

.ansi-magenta-intense-bg { background-color: rgb(160, 49, 150); }

.ansi-cyan-fg { color: rgb(96, 198, 200); }

.ansi-cyan-bg { background-color: rgb(96, 198, 200); }

.ansi-cyan-intense-fg { color: rgb(37, 143, 143); }

.ansi-cyan-intense-bg { background-color: rgb(37, 143, 143); }

.ansi-white-fg { color: rgb(197, 193, 180); }

.ansi-white-bg { background-color: rgb(197, 193, 180); }

.ansi-white-intense-fg { color: rgb(161, 166, 178); }

.ansi-white-intense-bg { background-color: rgb(161, 166, 178); }

.ansi-default-inverse-fg { color: rgb(255, 255, 255); }

.ansi-default-inverse-bg { background-color: rgb(0, 0, 0); }

.ansi-bold { font-weight: bold; }

.ansi-underline { text-decoration: underline; }

div.cell { -webkit-box-orient: vertical; -webkit-box-align: stretch; displa=
y: flex; flex-direction: column; align-items: stretch; border-radius: 2px; =
box-sizing: border-box; border-width: 1px; border-style: solid; border-colo=
r: transparent; width: 100%; padding: 5px; margin: 0px; outline: none; posi=
tion: relative; overflow: visible; }

div.cell::before { position: absolute; display: block; top: -1px; left: -1p=
x; width: 5px; height: calc(100% + 2px); content: ""; background: transpare=
nt; }

div.cell.jupyter-soft-selected { border-left-color: rgb(227, 242, 253); bor=
der-left-width: 1px; padding-left: 5px; border-right-color: rgb(227, 242, 2=
53); border-right-width: 1px; background: rgb(227, 242, 253); }

@media print {
  div.cell.jupyter-soft-selected { border-color: transparent; }
}

div.cell.selected, div.cell.selected.jupyter-soft-selected { border-color: =
rgb(171, 171, 171); }

div.cell.selected::before, div.cell.selected.jupyter-soft-selected::before =
{ position: absolute; display: block; top: -1px; left: -1px; width: 5px; he=
ight: calc(100% + 2px); content: ""; background: rgb(66, 165, 245); }

@media print {
  div.cell.selected, div.cell.selected.jupyter-soft-selected { border-color=
: transparent; }
}

.edit_mode div.cell.selected { border-color: rgb(102, 187, 106); }

.edit_mode div.cell.selected::before { position: absolute; display: block; =
top: -1px; left: -1px; width: 5px; height: calc(100% + 2px); content: ""; b=
ackground: rgb(102, 187, 106); }

@media print {
  .edit_mode div.cell.selected { border-color: transparent; }
}

.prompt { min-width: 14ex; padding: 0.4em; margin: 0px; font-family: monosp=
ace; text-align: right; line-height: 1.21429em; user-select: none; cursor: =
default; }

@media (max-width: 540px) {
  .prompt { text-align: left; }
}

div.inner_cell { min-width: 0px; -webkit-box-orient: vertical; -webkit-box-=
align: stretch; display: flex; flex-direction: column; align-items: stretch=
; -webkit-box-flex: 1; flex: 1 1 0%; }

div.input_area { border: 1px solid rgb(207, 207, 207); border-radius: 2px; =
background: rgb(247, 247, 247); line-height: 1.21429em; }

div.prompt:empty { padding-top: 0px; padding-bottom: 0px; }

div.unrecognized_cell { padding: 5px 5px 5px 0px; -webkit-box-orient: horiz=
ontal; -webkit-box-align: stretch; display: flex; flex-direction: row; alig=
n-items: stretch; }

div.unrecognized_cell .inner_cell { border-radius: 2px; padding: 5px; font-=
weight: bold; color: red; border: 1px solid rgb(207, 207, 207); background:=
 rgb(234, 234, 234); }

div.unrecognized_cell .inner_cell a { color: inherit; text-decoration: none=
; }

div.unrecognized_cell .inner_cell a:hover { color: inherit; text-decoration=
: none; }

@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt { display: none; }
}

div.code_cell { }

@media print {
  div.code_cell { break-inside: avoid; }
}

div.input { break-inside: avoid; -webkit-box-orient: horizontal; -webkit-bo=
x-align: stretch; display: flex; flex-direction: row; align-items: stretch;=
 }

@media (max-width: 540px) {
  div.input { -webkit-box-orient: vertical; -webkit-box-align: stretch; dis=
play: flex; flex-direction: column; align-items: stretch; }
}

div.prompt_container { display: flex; flex-direction: row; justify-content:=
 space-between; align-items: flex-start; text-align: right; }

div.input_prompt { color: rgb(48, 63, 159); border-top: 1px solid transpare=
nt; }

div.run_this_cell { display: none; cursor: pointer; color: rgb(51, 51, 51);=
 padding: 5px 2ex; width: 1ex; }

div.prompt { min-width: 15ex; }

@media (-moz-touch-enabled: 1), (any-pointer: coarse) {
  div.run_this_cell { display: block; }
}

div.input_area > div.highlight { margin: 0.4em; border: none; padding: 0px;=
 background-color: transparent; }

div.input_area > div.highlight > pre { margin: 0px; border: none; padding: =
0px; background-color: transparent; }

.CodeMirror { line-height: 1.21429em; font-size: 14px; height: auto; backgr=
ound: none; }

.CodeMirror-scroll { overflow: auto hidden; }

.CodeMirror-lines { padding: 0.4em 0px; }

.CodeMirror-linenumber { padding: 0px 8px 0px 4px; }

.CodeMirror-gutters { border-bottom-left-radius: 2px; border-top-left-radiu=
s: 2px; }

.CodeMirror pre { padding: 0px 0.4em; border: 0px; border-radius: 0px; }

.CodeMirror-cursor { border-left: 1.4px solid black; }

@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .CodeMirror-cursor { border-left: 2px solid black; }
}

@media screen and (min-width: 4320px) {
  .CodeMirror-cursor { border-left: 4px solid black; }
}

.highlight-base { color: rgb(0, 0, 0); }

.highlight-variable { color: rgb(0, 0, 0); }

.highlight-variable-2 { color: rgb(26, 26, 26); }

.highlight-variable-3 { color: rgb(51, 51, 51); }

.highlight-string { color: rgb(186, 33, 33); }

.highlight-comment { color: rgb(0, 121, 121); font-style: italic; }

.highlight-number { color: rgb(0, 136, 0); }

.highlight-atom { color: rgb(136, 136, 255); }

.highlight-keyword { color: rgb(0, 128, 0); font-weight: bold; }

.highlight-builtin { color: rgb(0, 128, 0); }

.highlight-error { color: rgb(255, 0, 0); }

.highlight-operator { color: rgb(170, 34, 255); font-weight: bold; }

.highlight-meta { color: rgb(170, 34, 255); }

.highlight-def { color: rgb(0, 0, 255); }

.highlight-string-2 { color: rgb(255, 85, 0); }

.highlight-qualifier { color: rgb(85, 85, 85); }

.highlight-bracket { color: rgb(153, 153, 119); }

.highlight-tag { color: rgb(17, 119, 0); }

.highlight-attribute { color: rgb(0, 0, 204); }

.highlight-header { color: blue; }

.highlight-quote { color: rgb(0, 153, 0); }

.highlight-link { color: rgb(0, 0, 204); }

.cm-s-ipython span.cm-keyword { color: rgb(0, 128, 0); font-weight: bold; }

.cm-s-ipython span.cm-atom { color: rgb(136, 136, 255); }

.cm-s-ipython span.cm-number { color: rgb(0, 136, 0); }

.cm-s-ipython span.cm-def { color: rgb(0, 0, 255); }

.cm-s-ipython span.cm-variable { color: rgb(0, 0, 0); }

.cm-s-ipython span.cm-operator { color: rgb(170, 34, 255); font-weight: bol=
d; }

.cm-s-ipython span.cm-variable-2 { color: rgb(26, 26, 26); }

.cm-s-ipython span.cm-variable-3 { color: rgb(51, 51, 51); }

.cm-s-ipython span.cm-comment { color: rgb(0, 121, 121); font-style: italic=
; }

.cm-s-ipython span.cm-string { color: rgb(186, 33, 33); }

.cm-s-ipython span.cm-string-2 { color: rgb(255, 85, 0); }

.cm-s-ipython span.cm-meta { color: rgb(170, 34, 255); }

.cm-s-ipython span.cm-qualifier { color: rgb(85, 85, 85); }

.cm-s-ipython span.cm-builtin { color: rgb(0, 128, 0); }

.cm-s-ipython span.cm-bracket { color: rgb(153, 153, 119); }

.cm-s-ipython span.cm-tag { color: rgb(17, 119, 0); }

.cm-s-ipython span.cm-attribute { color: rgb(0, 0, 204); }

.cm-s-ipython span.cm-header { color: blue; }

.cm-s-ipython span.cm-quote { color: rgb(0, 153, 0); }

.cm-s-ipython span.cm-link { color: rgb(0, 0, 204); }

.cm-s-ipython span.cm-error { color: rgb(255, 0, 0); }

.cm-s-ipython span.cm-tab { background: url("data:image/png;base64,iVBORw0K=
GgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFA=
QheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJ=
vElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=3D") righ=
t center no-repeat; }

div.output_wrapper { position: relative; -webkit-box-orient: vertical; -web=
kit-box-align: stretch; display: flex; flex-direction: column; align-items:=
 stretch; z-index: 1; }

div.output_scroll { height: 24em; width: 100%; overflow: auto; border-radiu=
s: 2px; box-shadow: rgba(0, 0, 0, 0.8) 0px 2px 8px inset; display: block; }

div.output_collapsed { margin: 0px; padding: 0px; -webkit-box-orient: verti=
cal; -webkit-box-align: stretch; display: flex; flex-direction: column; ali=
gn-items: stretch; }

div.out_prompt_overlay { height: 100%; padding: 0px 0.4em; position: absolu=
te; border-radius: 2px; }

div.out_prompt_overlay:hover { box-shadow: rgb(0, 0, 0) 0px 0px 1px inset; =
background: rgba(240, 240, 240, 0.5); }

div.output_prompt { color: rgb(216, 67, 21); }

div.output_area { padding: 0px; break-inside: avoid; -webkit-box-orient: ho=
rizontal; -webkit-box-align: stretch; display: flex; flex-direction: row; a=
lign-items: stretch; }

div.output_area .MathJax_Display { text-align: left !important; }

div.output_area .rendered_html table { margin-left: 0px; margin-right: 0px;=
 }

div.output_area .rendered_html img { margin-left: 0px; margin-right: 0px; }

div.output_area img, div.output_area svg { max-width: 100%; height: auto; }

div.output_area img.unconfined, div.output_area svg.unconfined { max-width:=
 none; }

div.output_area .mglyph > img { max-width: none; }

.output { -webkit-box-orient: vertical; -webkit-box-align: stretch; display=
: flex; flex-direction: column; align-items: stretch; }

@media (max-width: 540px) {
  div.output_area { -webkit-box-orient: vertical; -webkit-box-align: stretc=
h; display: flex; flex-direction: column; align-items: stretch; }
}

div.output_area pre { margin: 0px; padding: 1px 0px; border: 0px; vertical-=
align: baseline; color: black; background-color: transparent; border-radius=
: 0px; }

div.output_subarea { overflow-x: auto; padding: 0.4em; -webkit-box-flex: 1;=
 flex: 1 1 0%; max-width: calc(100% - 14ex); }

div.output_scroll div.output_subarea { overflow-x: visible; }

div.output_text { text-align: left; color: rgb(0, 0, 0); line-height: 1.214=
29em; }

div.output_stderr { background: rgb(255, 221, 221); }

div.output_latex { text-align: left; }

div.output_javascript:empty { padding: 0px; }

.js-error { color: darkred; }

div.raw_input_container { line-height: 1.21429em; padding-top: 5px; }

pre.raw_input_prompt { }

input.raw_input { font-family: monospace; font-size: inherit; color: inheri=
t; width: auto; vertical-align: baseline; padding: 0em 0.25em; margin: 0em =
0.25em; }

input.raw_input:focus { box-shadow: none; }

p.p-space { margin-bottom: 10px; }

div.output_unrecognized { padding: 5px; font-weight: bold; color: red; }

div.output_unrecognized a { color: inherit; text-decoration: none; }

div.output_unrecognized a:hover { color: inherit; text-decoration: none; }

div.output_text[dir=3D"rtl"] { text-align: right; }

.rendered_html { color: rgb(0, 0, 0); }

.rendered_html em { font-style: italic; }

.rendered_html strong { font-weight: bold; }

.rendered_html u { text-decoration: underline; }

.rendered_html :link { text-decoration: underline; }

.rendered_html :visited { text-decoration: underline; }

.rendered_html h1 { font-size: 185.7%; margin: 1.08em 0px 0px; font-weight:=
 bold; line-height: 1; }

.rendered_html h2 { font-size: 157.1%; margin: 1.27em 0px 0px; font-weight:=
 bold; line-height: 1; }

.rendered_html h3 { font-size: 128.6%; margin: 1.55em 0px 0px; font-weight:=
 bold; line-height: 1; }

.rendered_html h4 { font-size: 100%; margin: 2em 0px 0px; font-weight: bold=
; line-height: 1; }

.rendered_html h5 { font-size: 100%; margin: 2em 0px 0px; font-weight: bold=
; line-height: 1; font-style: italic; }

.rendered_html h6 { font-size: 100%; margin: 2em 0px 0px; font-weight: bold=
; line-height: 1; font-style: italic; }

.rendered_html h1:first-child { margin-top: 0.538em; }

.rendered_html h2:first-child { margin-top: 0.636em; }

.rendered_html h3:first-child { margin-top: 0.777em; }

.rendered_html h4:first-child { margin-top: 1em; }

.rendered_html h5:first-child { margin-top: 1em; }

.rendered_html h6:first-child { margin-top: 1em; }

.rendered_html ul:not(.list-inline), .rendered_html ol:not(.list-inline) { =
padding-left: 2em; }

.rendered_html ul { list-style: disc; }

.rendered_html ul ul { list-style: square; margin-top: 0px; }

.rendered_html ul ul ul { list-style: circle; }

.rendered_html ol { list-style: decimal; }

.rendered_html ol ol { list-style: upper-alpha; margin-top: 0px; }

.rendered_html ol ol ol { list-style: lower-alpha; }

.rendered_html ol ol ol ol { list-style: lower-roman; }

.rendered_html ol ol ol ol ol { list-style: decimal; }

.rendered_html * + ul { margin-top: 1em; }

.rendered_html * + ol { margin-top: 1em; }

.rendered_html hr { color: black; background-color: black; }

.rendered_html pre { margin: 1em 2em; padding: 0px; background-color: rgb(2=
55, 255, 255); }

.rendered_html code { background-color: rgb(239, 240, 241); }

.rendered_html p code { padding: 1px 5px; }

.rendered_html pre code { background-color: rgb(255, 255, 255); }

.rendered_html pre, .rendered_html code { border: 0px; color: rgb(0, 0, 0);=
 font-size: 100%; }

.rendered_html blockquote { margin: 1em 2em; }

.rendered_html table { margin-left: auto; margin-right: auto; border: none;=
 border-collapse: collapse; border-spacing: 0px; color: black; font-size: 1=
2px; table-layout: fixed; }

.rendered_html thead { border-bottom: 1px solid black; vertical-align: bott=
om; }

.rendered_html tr, .rendered_html th, .rendered_html td { text-align: right=
; vertical-align: middle; padding: 0.5em; line-height: normal; white-space:=
 normal; max-width: none; border: none; }

.rendered_html th { font-weight: bold; }

.rendered_html tbody tr:nth-child(2n+1) { background: rgb(245, 245, 245); }

.rendered_html tbody tr:hover { background: rgba(66, 165, 245, 0.2); }

.rendered_html * + table { margin-top: 1em; }

.rendered_html p { text-align: left; }

.rendered_html * + p { margin-top: 1em; }

.rendered_html img { display: block; margin-left: auto; margin-right: auto;=
 }

.rendered_html * + img { margin-top: 1em; }

.rendered_html img, .rendered_html svg { max-width: 100%; height: auto; }

.rendered_html img.unconfined, .rendered_html svg.unconfined { max-width: n=
one; }

.rendered_html .alert { margin-bottom: initial; }

.rendered_html * + .alert { margin-top: 1em; }

[dir=3D"rtl"] .rendered_html:not([dir=3D"ltr"]) p, .rendered_html[dir=3D"rt=
l"] p { text-align: right; }

div.text_cell { -webkit-box-orient: horizontal; -webkit-box-align: stretch;=
 display: flex; flex-direction: row; align-items: stretch; }

@media (max-width: 540px) {
  div.text_cell > div.prompt { display: none; }
}

div.text_cell_render { outline: none; resize: none; width: inherit; border-=
style: none; padding: 0.5em 0.5em 0.5em 0.4em; color: rgb(0, 0, 0); box-siz=
ing: border-box; }

a.anchor-link:link { text-decoration: none; padding: 0px 20px; visibility: =
hidden; }

h1:hover .anchor-link, h2:hover .anchor-link, h3:hover .anchor-link, h4:hov=
er .anchor-link, h5:hover .anchor-link, h6:hover .anchor-link { visibility:=
 visible; }

.text_cell.rendered .input_area { display: none; }

.text_cell.rendered .rendered_html { overflow: auto hidden; }

.text_cell.rendered .rendered_html tr, .text_cell.rendered .rendered_html t=
h, .text_cell.rendered .rendered_html td { max-width: none; }

.text_cell.unrendered .text_cell_render { display: none; }

.text_cell .dropzone .input_area { border: 2px dashed rgb(186, 186, 186); m=
argin: -1px; }

.cm-header-1, .cm-header-2, .cm-header-3, .cm-header-4, .cm-header-5, .cm-h=
eader-6 { font-weight: bold; font-family: "Helvetica Neue", Helvetica, Aria=
l, sans-serif; }

.cm-header-1 { font-size: 185.7%; }

.cm-header-2 { font-size: 157.1%; }

.cm-header-3 { font-size: 128.6%; }

.cm-header-4 { font-size: 110%; }

.cm-header-5 { font-size: 100%; font-style: italic; }

.cm-header-6 { font-size: 100%; font-style: italic; }

@media (max-width: 767px) {
  .notebook_app { padding-left: 0px; padding-right: 0px; }
}

#ipython-main-app { box-sizing: border-box; height: 100%; }

div#notebook_panel { margin: 0px; padding: 0px; box-sizing: border-box; hei=
ght: 100%; }

div#notebook { font-size: 14px; line-height: 20px; overflow: auto hidden; w=
idth: 100%; padding-top: 20px; padding-bottom: 20px; margin: 0px; outline: =
none; box-sizing: border-box; min-height: 100%; }

@media not print {
  #notebook-container { padding: 15px; background-color: rgb(255, 255, 255)=
; min-height: 0px; box-shadow: rgba(87, 87, 87, 0.2) 0px 0px 12px 1px; }
}

@media print {
  #notebook-container { width: 100%; }
}

div.ui-widget-content { border: 1px solid rgb(171, 171, 171); outline: none=
; }

pre.dialog { background-color: rgb(247, 247, 247); border: 1px solid rgb(22=
1, 221, 221); border-radius: 2px; padding: 0.4em 0.4em 0.4em 2em; }

p.dialog { padding: 0.2em; }

pre, code, kbd, samp { white-space: pre-wrap; }

#fonttest { font-family: monospace; }

p { margin-bottom: 0px; }

.end_space { min-height: 100px; transition: height 0.2s ease 0s; }

.notebook_app > #header { box-shadow: rgba(87, 87, 87, 0.2) 0px 0px 12px 1p=
x; }

@media not print {
  .notebook_app { background-color: rgb(238, 238, 238); }
}

kbd { border-style: solid; border-width: 1px; box-shadow: none; margin: 2px=
; padding: 1px 2px; }

.jupyter-keybindings { padding: 1px; line-height: 24px; border-bottom: 1px =
solid gray; }

.jupyter-keybindings input { margin: 0px; padding: 0px; border: none; }

.jupyter-keybindings i { padding: 6px; }

.well code { background-color: rgb(255, 255, 255); border-color: rgb(171, 1=
71, 171); border-width: 1px; border-style: solid; padding: 1px 2px; }

.celltoolbar { border-top: thin solid rgb(207, 207, 207); border-right: thi=
n solid rgb(207, 207, 207); border-left: thin solid rgb(207, 207, 207); bor=
der-image: initial; border-bottom: none; background: rgb(238, 238, 238); bo=
rder-radius: 2px 2px 0px 0px; width: 100%; height: 29px; padding-right: 4px=
; -webkit-box-orient: horizontal; -webkit-box-align: stretch; flex-directio=
n: row; align-items: stretch; -webkit-box-pack: end; justify-content: flex-=
end; display: -webkit-flex; }

@media print {
  .celltoolbar { display: none; }
}

.ctb_hideshow { display: none; vertical-align: bottom; }

.ctb_global_show .ctb_show.ctb_hideshow { display: block; }

.ctb_global_show .ctb_show + .input_area, .ctb_global_show .ctb_show + div.=
text_cell_input, .ctb_global_show .ctb_show ~ div.text_cell_render { border=
-top-right-radius: 0px; border-top-left-radius: 0px; }

.ctb_global_show .ctb_show ~ div.text_cell_render { border: 1px solid rgb(2=
07, 207, 207); }

.celltoolbar { font-size: 87%; padding-top: 3px; }

.celltoolbar select { color: rgb(85, 85, 85); background-color: rgb(255, 25=
5, 255); background-image: none; border: 1px solid rgb(204, 204, 204); box-=
shadow: rgba(0, 0, 0, 0.075) 0px 1px 1px inset; transition: border-color 0.=
15s ease-in-out 0s, box-shadow 0.15s ease-in-out 0s; line-height: 1.5; bord=
er-radius: 1px; width: inherit; font-size: inherit; height: 22px; padding: =
0px; display: inline-block; }

.celltoolbar select:focus { border-color: rgb(102, 175, 233); outline: 0px;=
 box-shadow: rgba(0, 0, 0, 0.075) 0px 1px 1px inset, rgba(102, 175, 233, 0.=
6) 0px 0px 8px; }

.celltoolbar select::-webkit-input-placeholder { color: rgb(153, 153, 153);=
 }

.celltoolbar select[disabled], .celltoolbar select[readonly], fieldset[disa=
bled] .celltoolbar select { background-color: rgb(238, 238, 238); opacity: =
1; }

.celltoolbar select[disabled], fieldset[disabled] .celltoolbar select { cur=
sor: not-allowed; }

textarea.celltoolbar select { height: auto; }

select.celltoolbar select { height: 30px; line-height: 30px; }

textarea.celltoolbar select, select[multiple].celltoolbar select { height: =
auto; }

.celltoolbar label { margin-left: 5px; margin-right: 5px; }

.tags_button_container { width: 100%; display: flex; }

.tag-container { display: flex; flex-direction: row; flex-grow: 1; overflow=
: hidden; position: relative; }

.tag-container > * { margin: 0px 4px; }

.remove-tag-btn { margin-left: 4px; }

.tags-input { display: flex; }

.cell-tag:last-child::after { content: ""; position: absolute; right: 0px; =
width: 40px; height: 100%; background: linear-gradient(to right, rgba(0, 0,=
 0, 0), rgb(238, 238, 238)); }

.tags-input > * { margin-left: 4px; }

.cell-tag, .tags-input input, .tags-input button { color: rgb(85, 85, 85); =
background-color: rgb(255, 255, 255); background-image: none; border: 1px s=
olid rgb(204, 204, 204); transition: border-color 0.15s ease-in-out 0s, box=
-shadow 0.15s ease-in-out 0s; border-radius: 1px; box-shadow: none; width: =
inherit; font-size: inherit; height: 22px; line-height: 22px; padding: 0px =
4px; display: inline-block; }

.cell-tag:focus, .tags-input input:focus, .tags-input button:focus { border=
-color: rgb(102, 175, 233); outline: 0px; box-shadow: rgba(0, 0, 0, 0.075) =
0px 1px 1px inset, rgba(102, 175, 233, 0.6) 0px 0px 8px; }

.cell-tag::-webkit-input-placeholder, .tags-input input::-webkit-input-plac=
eholder, .tags-input button::-webkit-input-placeholder { color: rgb(153, 15=
3, 153); }

.cell-tag[disabled], .tags-input input[disabled], .tags-input button[disabl=
ed], .cell-tag[readonly], .tags-input input[readonly], .tags-input button[r=
eadonly], fieldset[disabled] .cell-tag, fieldset[disabled] .tags-input inpu=
t, fieldset[disabled] .tags-input button { background-color: rgb(238, 238, =
238); opacity: 1; }

.cell-tag[disabled], .tags-input input[disabled], .tags-input button[disabl=
ed], fieldset[disabled] .cell-tag, fieldset[disabled] .tags-input input, fi=
eldset[disabled] .tags-input button { cursor: not-allowed; }

textarea.cell-tag, textarea.tags-input input, textarea.tags-input button { =
height: auto; }

select.cell-tag, select.tags-input input, select.tags-input button { height=
: 30px; line-height: 30px; }

textarea.cell-tag, textarea.tags-input input, textarea.tags-input button, s=
elect[multiple].cell-tag, select[multiple].tags-input input, select[multipl=
e].tags-input button { height: auto; }

.cell-tag, .tags-input button { padding: 0px 4px; }

.cell-tag { background-color: rgb(255, 255, 255); white-space: nowrap; }

.tags-input input[type=3D"text"]:focus { outline: none; box-shadow: none; b=
order-color: rgb(204, 204, 204); }

.completions { position: absolute; z-index: 110; overflow: hidden; border: =
1px solid rgb(171, 171, 171); border-radius: 2px; box-shadow: rgb(173, 173,=
 173) 0px 6px 10px -1px; line-height: 1; }

.completions select { background: white; outline: none; border: none; paddi=
ng: 0px; margin: 0px; overflow: auto; font-family: monospace; font-size: 11=
0%; color: rgb(0, 0, 0); width: auto; }

.completions select option.context { color: rgb(40, 96, 144); }

#kernel_logo_widget .current_kernel_logo { display: none; margin-top: -1px;=
 margin-bottom: -1px; width: 32px; height: 32px; }

[dir=3D"rtl"] #kernel_logo_widget { float: left !important; }

.modal .modal-body .move-path { display: flex; flex-direction: row; align-i=
tems: center; }

.modal .modal-body .move-path .server-root { padding-right: 20px; }

.modal .modal-body .move-path .path-input { flex: 1 1 0%; }

#menubar { box-sizing: border-box; margin-top: 1px; }

#menubar .navbar { border-top: 1px; border-radius: 0px 0px 2px 2px; margin-=
bottom: 0px; }

#menubar .navbar-toggle { float: left; padding-top: 7px; padding-bottom: 7p=
x; border: none; }

#menubar .navbar-collapse { clear: left; }

[dir=3D"rtl"] #menubar .navbar-toggle { float: right; }

[dir=3D"rtl"] #menubar .navbar-collapse { clear: right; }

[dir=3D"rtl"] #menubar .navbar-nav { float: right; }

[dir=3D"rtl"] #menubar .nav { padding-right: 0px; }

[dir=3D"rtl"] #menubar .navbar-nav > li { float: right; }

[dir=3D"rtl"] #menubar .navbar-right { float: left !important; }

ul.dropdown-menu:focus [dir=3D"rtl"] ul.dropdown-menu { text-align: right; =
left: auto; }

[dir=3D"rtl"] ul#new-menu.dropdown-menu { right: auto; left: 0px; }

.nav-wrapper { border-bottom: 1px solid rgb(231, 231, 231); }

i.menu-icon { padding-top: 4px; }

[dir=3D"rtl"] i.menu-icon.pull-right { float: left !important; }

ul.dropdown-menu li a.menu-shortcut-container { display: flex; flex-directi=
on: row; justify-content: space-between; align-items: flex-end; }

ul#help_menu li a { overflow: hidden; padding-right: 2.2em; }

ul#help_menu li a i { margin-right: -1.2em; }

[dir=3D"rtl"] ul#help_menu li a { padding-left: 2.2em; }

[dir=3D"rtl"] ul#help_menu li a i { margin-right: 0px; margin-left: -1.2em;=
 }

[dir=3D"rtl"] ul#help_menu li a i.pull-right { float: left !important; }

.dropdown-submenu { position: relative; }

.dropdown-submenu > .dropdown-menu { top: 0px; left: 100%; margin-top: -6px=
; margin-left: -1px; }

[dir=3D"rtl"] .dropdown-submenu > .dropdown-menu { right: 100%; margin-righ=
t: -1px; }

.dropdown-submenu:hover > .dropdown-menu { display: block; }

.dropdown-submenu > a::after { font-style: normal; font-variant: normal; fo=
nt-kerning: auto; font-optical-sizing: auto; font-feature-settings: normal;=
 font-variation-settings: normal; font-weight: normal; font-stretch: normal=
; line-height: 1; font-family: FontAwesome; font-size: inherit; text-render=
ing: auto; -webkit-font-smoothing: antialiased; display: block; content: "=
=EF=83=9A"; float: right; color: rgb(51, 51, 51); margin-top: 2px; margin-r=
ight: -10px; }

[dir=3D"rtl"] .dropdown-submenu > a::after { float: left; content: "=EF=83=
=99"; margin-right: 0px; margin-left: -10px; }

.dropdown-submenu:hover > a::after { color: rgb(38, 38, 38); }

.dropdown-submenu.pull-left { float: none; }

.dropdown-submenu.pull-left > .dropdown-menu { left: -100%; margin-left: 10=
px; }

.kb { color: darkgray; margin-left: 10px; text-transform: capitalize; }

.kb kbd { white-space: nowrap; }

#notification_area { z-index: 10; float: right !important; }

[dir=3D"rtl"] #notification_area { float: left !important; }

.indicator_area { color: rgb(86, 86, 86); margin-left: 5px; margin-right: 5=
px; z-index: 10; text-align: center; width: auto; float: right !important; =
}

[dir=3D"rtl"] .indicator_area { float: left !important; }

#kernel_indicator { color: rgb(86, 86, 86); margin-left: 5px; margin-right:=
 5px; z-index: 10; text-align: center; width: auto; border-left: 1px solid;=
 float: right !important; }

#kernel_indicator .kernel_indicator_name { padding-left: 5px; padding-right=
: 5px; color: rgb(16, 41, 48); }

[dir=3D"rtl"] #kernel_indicator { border-left: 0px; border-right: 1px solid=
; float: left !important; }

#modal_indicator { color: rgb(86, 86, 86); margin-left: 5px; margin-right: =
5px; z-index: 10; text-align: center; width: auto; float: right !important;=
 }

[dir=3D"rtl"] #modal_indicator { float: left !important; }

#readonly-indicator { color: rgb(86, 86, 86); z-index: 10; text-align: cent=
er; width: auto; margin: 2px 0px 0px; display: none; float: right !importan=
t; }

.modal_indicator::before { width: 1.28571em; text-align: center; }

.edit_mode .modal_indicator::before { display: inline-block; font-style: no=
rmal; font-variant: normal; font-kerning: auto; font-optical-sizing: auto; =
font-feature-settings: normal; font-variation-settings: normal; font-weight=
: normal; font-stretch: normal; line-height: 1; font-family: FontAwesome; f=
ont-size: inherit; text-rendering: auto; -webkit-font-smoothing: antialiase=
d; content: "=EF=81=80"; }

.command_mode .modal_indicator::before { display: inline-block; font-style:=
 normal; font-variant: normal; font-kerning: auto; font-optical-sizing: aut=
o; font-feature-settings: normal; font-variation-settings: normal; font-wei=
ght: normal; font-stretch: normal; line-height: 1; font-family: FontAwesome=
; font-size: inherit; text-rendering: auto; -webkit-font-smoothing: antiali=
ased; content: " "; }

.kernel_idle_icon::before { display: inline-block; font-style: normal; font=
-variant: normal; font-kerning: auto; font-optical-sizing: auto; font-featu=
re-settings: normal; font-variation-settings: normal; font-weight: normal; =
font-stretch: normal; line-height: 1; font-family: FontAwesome; font-size: =
inherit; text-rendering: auto; -webkit-font-smoothing: antialiased; content=
: "=EF=84=8C"; }

.kernel_busy_icon::before { display: inline-block; font-style: normal; font=
-variant: normal; font-kerning: auto; font-optical-sizing: auto; font-featu=
re-settings: normal; font-variation-settings: normal; font-weight: normal; =
font-stretch: normal; line-height: 1; font-family: FontAwesome; font-size: =
inherit; text-rendering: auto; -webkit-font-smoothing: antialiased; content=
: "=EF=84=91"; }

.kernel_dead_icon::before { display: inline-block; font-style: normal; font=
-variant: normal; font-kerning: auto; font-optical-sizing: auto; font-featu=
re-settings: normal; font-variation-settings: normal; font-weight: normal; =
font-stretch: normal; line-height: 1; font-family: FontAwesome; font-size: =
inherit; text-rendering: auto; -webkit-font-smoothing: antialiased; content=
: "=EF=87=A2"; }

.kernel_disconnected_icon::before { display: inline-block; font-style: norm=
al; font-variant: normal; font-kerning: auto; font-optical-sizing: auto; fo=
nt-feature-settings: normal; font-variation-settings: normal; font-weight: =
normal; font-stretch: normal; line-height: 1; font-family: FontAwesome; fon=
t-size: inherit; text-rendering: auto; -webkit-font-smoothing: antialiased;=
 content: "=EF=84=A7"; }

.notification_widget { z-index: 10; background: rgb(255, 255, 255); margin-=
right: 4px; color: rgb(51, 51, 51); border-color: rgb(204, 204, 204); }

.notification_widget:focus, .notification_widget.focus { color: rgb(51, 51,=
 51); background-color: rgb(230, 230, 230); border-color: rgb(140, 140, 140=
); }

.notification_widget:hover { color: rgb(51, 51, 51); background-color: rgb(=
230, 230, 230); border-color: rgb(173, 173, 173); }

.notification_widget:active, .notification_widget.active, .open > .dropdown=
-toggle.notification_widget { color: rgb(51, 51, 51); background-color: rgb=
(230, 230, 230); background-image: none; border-color: rgb(173, 173, 173); =
}

.notification_widget:active:hover, .notification_widget.active:hover, .open=
 > .dropdown-toggle.notification_widget:hover, .notification_widget:active:=
focus, .notification_widget.active:focus, .open > .dropdown-toggle.notifica=
tion_widget:focus, .notification_widget:active.focus, .notification_widget.=
active.focus, .open > .dropdown-toggle.notification_widget.focus { color: r=
gb(51, 51, 51); background-color: rgb(212, 212, 212); border-color: rgb(140=
, 140, 140); }

.notification_widget.disabled:hover, .notification_widget[disabled]:hover, =
fieldset[disabled] .notification_widget:hover, .notification_widget.disable=
d:focus, .notification_widget[disabled]:focus, fieldset[disabled] .notifica=
tion_widget:focus, .notification_widget.disabled.focus, .notification_widge=
t[disabled].focus, fieldset[disabled] .notification_widget.focus { backgrou=
nd-color: rgb(255, 255, 255); border-color: rgb(204, 204, 204); }

.notification_widget .badge { color: rgb(255, 255, 255); background-color: =
rgb(51, 51, 51); }

.notification_widget.warning { color: rgb(255, 255, 255); background-color:=
 rgb(180, 97, 2); border-color: rgb(180, 97, 2); }

.notification_widget.warning:focus, .notification_widget.warning.focus { co=
lor: rgb(255, 255, 255); background-color: rgb(236, 151, 31); border-color:=
 rgb(152, 95, 13); }

.notification_widget.warning:hover { color: rgb(255, 255, 255); background-=
color: rgb(236, 151, 31); border-color: rgb(213, 133, 18); }

.notification_widget.warning:active, .notification_widget.warning.active, .=
open > .dropdown-toggle.notification_widget.warning { color: rgb(255, 255, =
255); background-color: rgb(236, 151, 31); background-image: none; border-c=
olor: rgb(213, 133, 18); }

.notification_widget.warning:active:hover, .notification_widget.warning.act=
ive:hover, .open > .dropdown-toggle.notification_widget.warning:hover, .not=
ification_widget.warning:active:focus, .notification_widget.warning.active:=
focus, .open > .dropdown-toggle.notification_widget.warning:focus, .notific=
ation_widget.warning:active.focus, .notification_widget.warning.active.focu=
s, .open > .dropdown-toggle.notification_widget.warning.focus { color: rgb(=
255, 255, 255); background-color: rgb(213, 133, 18); border-color: rgb(152,=
 95, 13); }

.notification_widget.warning.disabled:hover, .notification_widget.warning[d=
isabled]:hover, fieldset[disabled] .notification_widget.warning:hover, .not=
ification_widget.warning.disabled:focus, .notification_widget.warning[disab=
led]:focus, fieldset[disabled] .notification_widget.warning:focus, .notific=
ation_widget.warning.disabled.focus, .notification_widget.warning[disabled]=
.focus, fieldset[disabled] .notification_widget.warning.focus { background-=
color: rgb(240, 173, 78); border-color: rgb(238, 162, 54); }

.notification_widget.warning .badge { color: rgb(240, 173, 78); background-=
color: rgb(255, 255, 255); }

.notification_widget.success { color: rgb(255, 255, 255); background-color:=
 rgb(92, 184, 92); border-color: rgb(76, 174, 76); }

.notification_widget.success:focus, .notification_widget.success.focus { co=
lor: rgb(255, 255, 255); background-color: rgb(68, 157, 68); border-color: =
rgb(37, 86, 37); }

.notification_widget.success:hover { color: rgb(255, 255, 255); background-=
color: rgb(68, 157, 68); border-color: rgb(57, 132, 57); }

.notification_widget.success:active, .notification_widget.success.active, .=
open > .dropdown-toggle.notification_widget.success { color: rgb(255, 255, =
255); background-color: rgb(68, 157, 68); background-image: none; border-co=
lor: rgb(57, 132, 57); }

.notification_widget.success:active:hover, .notification_widget.success.act=
ive:hover, .open > .dropdown-toggle.notification_widget.success:hover, .not=
ification_widget.success:active:focus, .notification_widget.success.active:=
focus, .open > .dropdown-toggle.notification_widget.success:focus, .notific=
ation_widget.success:active.focus, .notification_widget.success.active.focu=
s, .open > .dropdown-toggle.notification_widget.success.focus { color: rgb(=
255, 255, 255); background-color: rgb(57, 132, 57); border-color: rgb(37, 8=
6, 37); }

.notification_widget.success.disabled:hover, .notification_widget.success[d=
isabled]:hover, fieldset[disabled] .notification_widget.success:hover, .not=
ification_widget.success.disabled:focus, .notification_widget.success[disab=
led]:focus, fieldset[disabled] .notification_widget.success:focus, .notific=
ation_widget.success.disabled.focus, .notification_widget.success[disabled]=
.focus, fieldset[disabled] .notification_widget.success.focus { background-=
color: rgb(92, 184, 92); border-color: rgb(76, 174, 76); }

.notification_widget.success .badge { color: rgb(92, 184, 92); background-c=
olor: rgb(255, 255, 255); }

.notification_widget.info { color: rgb(255, 255, 255); background-color: rg=
b(91, 192, 222); border-color: rgb(70, 184, 218); }

.notification_widget.info:focus, .notification_widget.info.focus { color: r=
gb(255, 255, 255); background-color: rgb(49, 176, 213); border-color: rgb(2=
7, 109, 133); }

.notification_widget.info:hover { color: rgb(255, 255, 255); background-col=
or: rgb(49, 176, 213); border-color: rgb(38, 154, 188); }

.notification_widget.info:active, .notification_widget.info.active, .open >=
 .dropdown-toggle.notification_widget.info { color: rgb(255, 255, 255); bac=
kground-color: rgb(49, 176, 213); background-image: none; border-color: rgb=
(38, 154, 188); }

.notification_widget.info:active:hover, .notification_widget.info.active:ho=
ver, .open > .dropdown-toggle.notification_widget.info:hover, .notification=
_widget.info:active:focus, .notification_widget.info.active:focus, .open > =
.dropdown-toggle.notification_widget.info:focus, .notification_widget.info:=
active.focus, .notification_widget.info.active.focus, .open > .dropdown-tog=
gle.notification_widget.info.focus { color: rgb(255, 255, 255); background-=
color: rgb(38, 154, 188); border-color: rgb(27, 109, 133); }

.notification_widget.info.disabled:hover, .notification_widget.info[disable=
d]:hover, fieldset[disabled] .notification_widget.info:hover, .notification=
_widget.info.disabled:focus, .notification_widget.info[disabled]:focus, fie=
ldset[disabled] .notification_widget.info:focus, .notification_widget.info.=
disabled.focus, .notification_widget.info[disabled].focus, fieldset[disable=
d] .notification_widget.info.focus { background-color: rgb(91, 192, 222); b=
order-color: rgb(70, 184, 218); }

.notification_widget.info .badge { color: rgb(91, 192, 222); background-col=
or: rgb(255, 255, 255); }

.notification_widget.danger { color: rgb(255, 255, 255); background-color: =
rgb(223, 4, 4); border-color: rgb(223, 4, 4); }

.notification_widget.danger:focus, .notification_widget.danger.focus { colo=
r: rgb(255, 255, 255); background-color: rgb(201, 48, 44); border-color: rg=
b(118, 28, 25); }

.notification_widget.danger:hover { color: rgb(255, 255, 255); background-c=
olor: rgb(201, 48, 44); border-color: rgb(172, 41, 37); }

.notification_widget.danger:active, .notification_widget.danger.active, .op=
en > .dropdown-toggle.notification_widget.danger { color: rgb(255, 255, 255=
); background-color: rgb(201, 48, 44); background-image: none; border-color=
: rgb(172, 41, 37); }

.notification_widget.danger:active:hover, .notification_widget.danger.activ=
e:hover, .open > .dropdown-toggle.notification_widget.danger:hover, .notifi=
cation_widget.danger:active:focus, .notification_widget.danger.active:focus=
, .open > .dropdown-toggle.notification_widget.danger:focus, .notification_=
widget.danger:active.focus, .notification_widget.danger.active.focus, .open=
 > .dropdown-toggle.notification_widget.danger.focus { color: rgb(255, 255,=
 255); background-color: rgb(172, 41, 37); border-color: rgb(118, 28, 25); =
}

.notification_widget.danger.disabled:hover, .notification_widget.danger[dis=
abled]:hover, fieldset[disabled] .notification_widget.danger:hover, .notifi=
cation_widget.danger.disabled:focus, .notification_widget.danger[disabled]:=
focus, fieldset[disabled] .notification_widget.danger:focus, .notification_=
widget.danger.disabled.focus, .notification_widget.danger[disabled].focus, =
fieldset[disabled] .notification_widget.danger.focus { background-color: rg=
b(217, 83, 79); border-color: rgb(212, 63, 58); }

.notification_widget.danger .badge { color: rgb(217, 83, 79); background-co=
lor: rgb(255, 255, 255); }

div#pager { background-color: rgb(255, 255, 255); font-size: 14px; line-hei=
ght: 20px; overflow: hidden; display: none; position: fixed; bottom: 0px; w=
idth: 100%; max-height: 50%; padding-top: 8px; box-shadow: rgba(87, 87, 87,=
 0.2) 0px 0px 12px 1px; z-index: 100; top: auto !important; }

div#pager pre { line-height: 1.21429em; color: rgb(0, 0, 0); background-col=
or: rgb(247, 247, 247); padding: 0.4em; }

div#pager #pager-button-area { position: absolute; top: 8px; right: 20px; }

div#pager #pager-button-area .ui-button { padding: 0px 10px; }

div#pager #pager-contents { position: relative; overflow: auto; width: 100%=
; height: 100%; }

div#pager #pager-contents #pager-container { position: relative; padding: 1=
5px 0px; box-sizing: border-box; }

div#pager .ui-resizable-handle { top: 0px; height: 8px; background: rgb(247=
, 247, 247); border-top: 1px solid rgb(207, 207, 207); border-bottom: 1px s=
olid rgb(207, 207, 207); }

div#pager .ui-resizable-handle::after { content: ""; top: 2px; left: 50%; h=
eight: 3px; width: 30px; margin-left: -15px; position: absolute; border-top=
: 1px solid rgb(207, 207, 207); }

.quickhelp { -webkit-box-orient: horizontal; -webkit-box-align: stretch; di=
splay: flex; flex-direction: row; align-items: stretch; line-height: 1.8em;=
 }

.shortcut_key { display: inline-block; width: 21ex; text-align: right; font=
-family: monospace; }

.shortcut_descr { display: inline-block; -webkit-box-flex: 1; flex: 1 1 0%;=
 }

span.save_widget { height: 30px; margin-top: 4px; display: flex; justify-co=
ntent: flex-start; align-items: baseline; width: 50%; flex: 1 1 0%; }

span.save_widget span.filename { height: 100%; line-height: 1em; margin-lef=
t: 16px; border: none; font-size: 146.5%; text-overflow: ellipsis; overflow=
: hidden; white-space: nowrap; border-radius: 2px; }

span.save_widget span.filename:hover { background-color: rgb(230, 230, 230)=
; }

[dir=3D"rtl"] span.save_widget.pull-left { float: right !important; }

[dir=3D"rtl"] span.save_widget span.filename { margin-left: 0px; margin-rig=
ht: 16px; }

span.checkpoint_status, span.autosave_status { font-size: small; white-spac=
e: nowrap; padding: 0px 5px; }

@media (max-width: 767px) {
  span.save_widget { font-size: small; padding: 0px 0px 0px 5px; }
  span.checkpoint_status, span.autosave_status { display: none; }
}

@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status { display: none; }
  span.autosave_status { font-size: x-small; }
}

.toolbar { padding: 0px; margin-left: -5px; margin-top: 2px; margin-bottom:=
 5px; box-sizing: border-box; }

.toolbar select, .toolbar label { width: auto; vertical-align: middle; marg=
in-bottom: 0px; display: inline; font-size: 92%; margin-left: 0.3em; margin=
-right: 0.3em; padding: 3px 0px 0px; }

.toolbar .btn { padding: 2px 8px; }

.toolbar .btn-group { margin-top: 0px; margin-left: 5px; }

.toolbar-btn-label { margin-left: 6px; }

#maintoolbar { margin-bottom: -3px; margin-top: -8px; border: 0px; min-heig=
ht: 27px; margin-left: 0px; padding-top: 11px; padding-bottom: 3px; }

#maintoolbar .navbar-text { float: none; vertical-align: middle; text-align=
: right; margin-left: 5px; margin-right: 0px; margin-top: 0px; }

.select-xs { height: 24px; }

[dir=3D"rtl"] .btn-group > .btn, .btn-group-vertical > .btn { float: right;=
 }

.pulse, .dropdown-menu > li > a.pulse, li.pulse > a.dropdown-toggle, li.pul=
se.open > a.dropdown-toggle { background-color: rgb(243, 118, 38); color: w=
hite; }

@-webkit-keyframes fadeOut {=20
  0% { opacity: 1; }
  100% { opacity: 0; }
}

@-webkit-keyframes fadeIn {=20
  0% { opacity: 0; }
  100% { opacity: 1; }
}

.bigtooltip { overflow: auto; height: 200px; transition-property: height; t=
ransition-duration: 500ms; }

.smalltooltip { transition-property: height; transition-duration: 500ms; te=
xt-overflow: ellipsis; overflow: hidden; height: 85px; }

.tooltipbuttons { position: absolute; padding-right: 15px; top: 0px; right:=
 0px; }

.tooltipbuttons .ui-button { padding: 0px 10px; }

.tooltiptext { padding-right: 30px; padding-top: 5px; }

.ipython_tooltip { max-width: 700px; animation: 400ms ease 0s 1 normal none=
 running fadeIn; vertical-align: middle; background-color: rgb(247, 247, 24=
7); overflow: visible; border: 1px solid rgb(171, 171, 171); outline: none;=
 padding: 3px 3px 3px 7px; margin: 0px; font-family: monospace; min-height:=
 50px; box-shadow: rgb(173, 173, 173) 0px 6px 10px -1px; border-radius: 2px=
; position: absolute; z-index: 1000; }

.ipython_tooltip a { float: right; }

.ipython_tooltip .tooltiptext pre { border: 0px; border-radius: 0px; font-s=
ize: 100%; background-color: rgb(247, 247, 247); }

.pretooltiparrow { left: 0px; margin: 0px; top: -16px; width: 40px; height:=
 16px; overflow: hidden; position: absolute; }

.pretooltiparrow::before { background-color: rgb(247, 247, 247); border: 1p=
x solid rgb(171, 171, 171); z-index: 11; content: ""; position: absolute; l=
eft: 15px; top: 10px; width: 25px; height: 25px; transform: rotate(45deg); =
}

div.typeahead__container { font: revert; }

ul.typeahead__list i { width: 18px; }

ul.typeahead__list { max-height: 80vh; overflow: auto; }

ul.typeahead__list > li > a { white-space: normal; }

ul.typeahead__list > li > a.pull-right { float: left !important; }

[dir=3D"rtl"] .typeahead__list { text-align: right; }

.cmd-palette .modal-body { padding: 7px; }

.cmd-palette form { background: white; }

.cmd-palette input { outline: none; }

.no-shortcut { min-width: 20px; color: transparent; }

[dir=3D"rtl"] .no-shortcut.pull-right { float: left !important; }

[dir=3D"rtl"] .command-shortcut.pull-right { float: left !important; }

.command-shortcut::before { content: "(command mode)"; padding-right: 3px; =
color: rgb(119, 119, 119); }

.edit-shortcut::before { content: "(edit)"; padding-right: 3px; color: rgb(=
119, 119, 119); }

[dir=3D"rtl"] .edit-shortcut.pull-right { float: left !important; }

#find-and-replace #replace-preview .match, #find-and-replace #replace-previ=
ew .insert { background-color: rgb(187, 222, 251); border-color: rgb(144, 2=
02, 249); border-style: solid; border-width: 1px; border-radius: 0px; }

[dir=3D"ltr"] #find-and-replace .input-group-btn + .form-control { border-l=
eft: none; }

[dir=3D"rtl"] #find-and-replace .input-group-btn + .form-control { border-r=
ight: none; }

#find-and-replace #replace-preview .replace .match { background-color: rgb(=
255, 205, 210); border-color: rgb(239, 154, 154); border-radius: 0px; }

#find-and-replace #replace-preview .replace .insert { background-color: rgb=
(200, 230, 201); border-color: rgb(165, 214, 167); border-radius: 0px; }

#find-and-replace #replace-preview { max-height: 60vh; overflow: auto; }

#find-and-replace #replace-preview pre { padding: 5px 10px; }

.terminal-app { background: rgb(238, 238, 238); }

.terminal-app #header { background: rgb(255, 255, 255); box-shadow: rgba(87=
, 87, 87, 0.2) 0px 0px 12px 1px; }

.terminal-app .terminal { width: 100%; float: left; font-family: monospace;=
 color: white; background: black; padding: 0.4em; border-radius: 2px; box-s=
hadow: rgba(87, 87, 87, 0.4) 0px 0px 12px 1px; line-height: 1em; font-size:=
 14px; }

.terminal-app .terminal .xterm-rows { padding: 10px; }

.terminal-app .terminal-cursor { color: black; background: white; }

.terminal-app .terminado-container-container { padding-top: 20px; height: 1=
00%; }

.terminal-app #terminado-container { height: 100%; }

.btn-danger { color: rgb(255, 255, 255); background-color: rgb(223, 4, 4); =
border-color: rgb(223, 4, 4); }

.btn-warning { color: rgb(255, 255, 255); background-color: rgb(180, 97, 2)=
; border-color: rgb(180, 97, 2); }

.close { float: right; font-size: 19.5px; font-weight: bold; line-height: 1=
; color: rgb(0, 0, 0); text-shadow: rgb(255, 255, 255) 0px 1px 0px; opacity=
: 0.6; }

.close:hover, .close:focus { color: rgb(0, 0, 0); text-decoration: none; cu=
rsor: pointer; opacity: 1; }

button.close { padding: 0px; cursor: pointer; background: transparent; bord=
er: 0px; appearance: none; }

.navbar-nav > li > a { color: rgb(86, 86, 86); }

.navbar-nav > li > a:focus { outline: -webkit-focus-ring-color auto 5px; }

.menu_focus_highlight a:focus { outline: -webkit-focus-ring-color auto 5px;=
 }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/static/notebook/css/override.css?v=16733f6ba5f2224692fe4e654f3cbb2e3cae82f1df06ca53aa1cb88b147465f16c968c0898e2b0203a7ad3a469f82b959e26bb4b27b790f7f364c4336449b0aa

@charset "utf-8";

#ipython-main-app { position: relative; }
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: text/css
Content-Transfer-Encoding: quoted-printable
Content-Location: http://localhost:8890/custom/custom.css

@charset "utf-8";
=0A
------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: image/png
Content-Transfer-Encoding: base64
Content-Location: http://localhost:8890/static/base/images/logo.png?v=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

------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN----
Content-Type: image/png
Content-Transfer-Encoding: base64
Content-Location: http://localhost:8890/kernelspecs/python3/logo-64x64.png

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
bn8AAAAASUVORK5CYII=

------MultipartBoundary--HlNdHZJKXCuSY8T0at0L171aOQqHLPDiGOUky0MuaN------
ter Notebook-table1.mhtml…]()


The mse of the (Low, High) forcasting is
[0.004799886196411286, 0.0032559867677543057]

















22  02-23-2024  1.2679  1.2659  1.2702  1.2648
