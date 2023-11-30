---
layout: about
title: about
permalink: /
order: a
subtitle: #x

news: false  # includes a list of news items
social: true  # includes social icons at the bottom of the page
---

# Islesboro wins $100k DOE Rural Energy Prize and enters Round 2 of Prize Competition
<br />
Islesboro won the U.S. Department of Energy's <a href="https://www.herox.com/rural-energy/teams">Energizing Rural Communities Prize!</a>

With these funds, we will build our capacity to offer logistical support to Islesboro residents and organizations who want solar, insulation, heat pumps, and other energy upgrades. We will also be able to apply for additional funding to reduce the upfront cost of clean energy projects on the island. 
<br />

<div class="row card-intro">
    <div class="col-sm mt-1 mt-md-0">
      <div class="card-item card-yellow">
        <a class="button card-yellow col-sm" href="https://forms.gle/y4oqnhghc7WWJ97bA">
          <span class="buttonLarge">Sign up for a free Home Energy Assessment <i class="fa-solid fa-circle-arrow-right"></i></span>
        </a>
      </div>
    </div>
</div>

<div class="row card-intro">
    <div class="col-sm mt-2 mt-md-0">
      <div class="card-item card-yellow">
        <h2>Say Hello to Islesboro's Community Energy Coordinator!</h2>
        <p>Kizzi Barton has joined the Rural Energy Prize team as Islesboro's first Coordinator</p>
        <a class="button card-yellow" href="https://islesboroenergy.org/coordinator/">Meet the Coordinator <i class="fa-solid fa-circle-arrow-right"></i></a>
      </div>
    </div>
    <div class="col-sm mt-2 mt-md-0">
      <div class="card-item card-blue">
        <h2>Residents and Friends: Tell us about your home energy needs</h2>
        <p>Tell us what energy-related needs and ideas you have for the island and your homes</p>
            <a class="button card-yellow" href="https://forms.gle/ExXFmbJW7C8rVzrC9">Take our survey <i class="fa-solid fa-circle-arrow-right"></i></a>
      </div>
    </div>
</div>

<br />
<div>
    <h2>Watch the Islesboro Prize Plan introductory video:</h2>
    <div style="padding: 5px" />
    <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/852559307?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" style="position:absolute;top:0;left:0;width:100%;height:100%;border-radius:8px;" title="Islesboro Rural Energy Prize - Info Meeting"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
</div>
<br />

# News
          
<div class="news">
  {% if site.news != blank -%} 
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
    {%- assign news = site.news | reverse -%} 
    {% for item in news limit: site.news_limit %} 
      <tr>
        <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
        <td>
          {% if item.inline -%} 
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
          {%- else -%} 
            <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
          {%- endif %} 
        </td>
      </tr>
    {%- endfor %} 
    </table>
  </div>
{%- else -%} 
  <p>No news so far...</p>
{%- endif %} 
</div>

<br />


<div class="row justify-content-sm-center">
  <hr width="100%" />
</div>

<div class="row justify-content-sm-center">
  <hr>
  <div class="col-sm-2 col-md-0"></div>
  <div class="col-sm-8 col-md-0">
        <!-- Begin Mailchimp Signup Form -->
        <link href="//cdn-images.mailchimp.com/embedcode/classic-10_7_dtp.css" rel="stylesheet" type="text/css">
        <style type="text/css">
        	#mc_embed_signup{background:#fff; clear:both; font:14px; text-align:center; align-items:center;}
          #mc_embed_signup form {text-align:center; padding:0px;}
        	#mc_heading{font-weight: 300; font-size: 1.3em; line-height: 1.0em; padding:10px 0px;}
          #mc_label{font-weight: 300; font-size: 0.8em;}
          #mc_embed_signup .mc-field-group {position:relative; width:100%; padding-bottom:3%; min-height:50px;}
          #mc_embed_signup div#mce-responses {float:center; top:-1.4em; padding:0em .5em 0em .5em; overflow:hidden; width:100%; margin: 0 5%; clear: both;}
          #mc_embed_signup .footer {width:100%; align-items: center;}
          #mc_embed_signup .brandingLogo {justify-self:center;}
          #mc-embedded-subscribe {clear:both; width:auto; display:block; margin:0;}
        </style>
        <div id="mc_embed_signup">
          <form action="https://islesboroenergy.us14.list-manage.com/subscribe/post?u=07fbabaf1bf18f715f917a219&amp;id=f2f1418c65" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
            <div id="mc_embed_signup_scroll">
              <div style="height: 10px" />
            	 <span id="mc_heading">SIGN UP FOR ISLESBORO ENERGY NEWS & UPDATES</span>
               <div style="height: 10px" />
                <div class="mc-field-group">
                	<label id="mc_label" for="mce-EMAIL">EMAIL ADDRESS</label>
                	<input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
                </div>
                <div hidden="true"><input type="hidden" name="tags" value="7258151"></div>
                	<div id="mce-responses" class="clear foot">
                		<div class="response" id="mce-error-response" style="display:none"></div>
                		<div class="response" id="mce-success-response" style="display:none"></div>
                	</div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
                    <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_07fbabaf1bf18f715f917a219_f2f1418c65" tabindex="-1" value=""></div>
                        <div class="optionalParent">
                            <div class="clear footer">
                                <input type="submit" value="SUBSCRIBE" name="subscribe" id="mc-embedded-subscribe" class="button" style="align:center">
                                <br>
                                <p class="brandingLogo"><a href="http://eepurl.com/hWzSSD" title="Mailchimp - email marketing made easy and fun"><img src="https://eep.io/mc-cdn-images/template_images/branding_logo_text_dark_dtp.svg"></a></p>
                            </div>
                        </div>
                    </div>
                </form>
            </div>
        <script type='text/javascript' src='//s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js'></script><script type='text/javascript'>(function($) {window.fnames = new Array(); window.ftypes = new Array();fnames[0]='EMAIL';ftypes[0]='email';fnames[1]='FNAME';ftypes[1]='text';fnames[2]='LNAME';ftypes[2]='text';fnames[3]='ADDRESS';ftypes[3]='address';fnames[4]='PHONE';ftypes[4]='phone';fnames[5]='BIRTHDAY';ftypes[5]='birthday';}(jQuery));var $mcj = jQuery.noConflict(true);</script>
        <!--End mc_embed_signup-->
    </div>
    <div class="col-sm-2 col-md-0"></div>

</div>


<!-- Energy Jamboree Banner section -->
<!--div class="row justify-content-sm-center">
    <div class="col-sm-2 col-md-0"></div>
    <div class="col-sm-8 col-md-0">
      <a href="https://forms.gle/sdhgGq9oNAGYJ6eZA" style="text-decoration: none">
        <img src="{{ site.url }}/assets/img/jamboree_ev_ride_web.svg" alt="Jamboree EV rides signup" class="img-fluid-svg" />
      </a>
      <br />
      <br />
      <a href="https://forms.gle/MXj4Cdsj8strL2J26" style="text-decoration: none">
        <img src="{{ site.url }}/assets/img/jamboree_survey_web.svg" alt="Home Energy and Jamboree Survey" class="img-fluid-svg" />
      </a>
      <div style="height: 20px" />
        <a href="jamboree/" style="text-decoration: none">
          <img src="{{ site.url }}/assets/img/jamboree_flyer_web.svg" alt="Jamboree flyer" class="img-fluid-svg" />
        </a>
        <div style="height: 20px" />
        <div style="width:100%;align-items:center;justify-content:center;display:flex">
        	<div style="width:50%">
        		  <img src="{{ site.url }}/assets/img/icc_logo_color_rev.jpg" alt="Jamboree flyer" class="img-fluid-svg" />
        	</div>
        </div>
        <div style="height: 20px" />
        <a href="https://fb.me/e/2PAxxLDHL" style="text-decoration: none">
          <img src="{{ site.url }}/assets/img/jamboree_button_fb_horiz_web.png" alt="Jamboree flyer" class="img-fluid-svg" />
        </a>
        <div style="height: 20px" />
        <a href="mailto:jamboree@islesboroenergy.org?subject=Website" style="text-decoration: none">
          <img src="{{ site.url }}/assets/img/jamboree_button_email_horiz_web.png" alt="Jamboree flyer" class="img-fluid-svg" />
        </a>
        <div style="height: 20px" />
    </div>
    <div class="col-sm-2 col-md-0"></div>
</div-->