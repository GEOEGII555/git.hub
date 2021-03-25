<!DOCTYPE html>
<html lang="en"><head>
  
  <meta charset="utf-8">
  <title>Creating a GitHub Pages site - GitHub Docs</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="alternate icon" type="image/png" href="/assets/images/site/favicon.png">
  <link rel="icon" type="image/svg+xml" href="/assets/images/site/favicon.svg">
  <link rel="stylesheet" href="/dist/index.css?hash=13efac4ac3fbe41655bb613c291169aa">

  
  
    <meta name="description" content="You can create a GitHub Pages site in a new or existing repository.">
  
  
    <meta name="keywords" content="pages">
  
  
  
    <link rel="alternate" hreflang="en" href="https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site">
  
    <link rel="alternate" hreflang="zh-Hans" href="https://docs.github.com/cn/github/working-with-github-pages/creating-a-github-pages-site">
  
    <link rel="alternate" hreflang="ja" href="https://docs.github.com/ja/github/working-with-github-pages/creating-a-github-pages-site">
  
    <link rel="alternate" hreflang="es" href="https://docs.github.com/es/github/working-with-github-pages/creating-a-github-pages-site">
  
    <link rel="alternate" hreflang="pt" href="https://docs.github.com/pt/github/working-with-github-pages/creating-a-github-pages-site">
  
    <link rel="alternate" hreflang="de" href="https://docs.github.com/de/github/working-with-github-pages/creating-a-github-pages-site">
  
  <meta name="google-site-verification" content="OgdQc0GZfjDI52wDv1bkMT-SLpBUo_h5nn9mI9L22xQ">
  <meta name="google-site-verification" content="c1kuD-K2HIVF635lypcsWPoD4kilo5-jA_wBFyT4uMY">

  
  <meta name="csrf-token" content="W7qzLwbw-38GsrhYAQw0LvDCTuoUFS_UNaL0">
  <meta name="site.data.ui.search.placeholder" content="Search topics, products...">
<meta name="shimejiBrowserExtensionId" content="gohjpllcolmccldfdggmamodembldgpc" data-version="1.6.5"><style type="text/css">
@charset "UTF-8";
/*!
 * jQuery contextMenu - Plugin for simple contextMenu handling
 *
 * Version: v2.5.0
 *
 * Authors: Björn Brala (SWIS.nl), Rodney Rehm, Addy Osmani (patches for FF)
 * Web: http://swisnl.github.io/jQuery-contextMenu/
 *
 * Copyright (c) 2011-2017 SWIS BV and contributors
 *
 * Licensed under
 *   MIT License http://www.opensource.org/licenses/mit-license
 *
 * Date: 2017-05-25T11:30:28.663Z
 */
@-webkit-keyframes cm-spin {
  0% {
    -webkit-transform: translateY(-50%) rotate(0deg);
            transform: translateY(-50%) rotate(0deg);
  }
  100% {
    -webkit-transform: translateY(-50%) rotate(359deg);
            transform: translateY(-50%) rotate(359deg);
  }
}
@-o-keyframes cm-spin {
  0% {
    -webkit-transform: translateY(-50%) rotate(0deg);
         -o-transform: translateY(-50%) rotate(0deg);
            transform: translateY(-50%) rotate(0deg);
  }
  100% {
    -webkit-transform: translateY(-50%) rotate(359deg);
         -o-transform: translateY(-50%) rotate(359deg);
            transform: translateY(-50%) rotate(359deg);
  }
}
@keyframes cm-spin {
  0% {
    -webkit-transform: translateY(-50%) rotate(0deg);
         -o-transform: translateY(-50%) rotate(0deg);
            transform: translateY(-50%) rotate(0deg);
  }
  100% {
    -webkit-transform: translateY(-50%) rotate(359deg);
         -o-transform: translateY(-50%) rotate(359deg);
            transform: translateY(-50%) rotate(359deg);
  }
}

@font-face {
  font-family: "context-menu-icons";
  font-style: normal;
  font-weight: normal;

  src: url("font/context-menu-icons.eot?4yg1f");
  src: url("font/context-menu-icons.eot?4yg1f#iefix") format("embedded-opentype"), url("font/context-menu-icons.woff2?4yg1f") format("woff2"), url("font/context-menu-icons.woff?4yg1f") format("woff"), url("font/context-menu-icons.ttf?4yg1f") format("truetype");
}

.context-menu-icon-add:before {
  content: "EA01";
}

.context-menu-icon-copy:before {
  content: "EA02";
}

.context-menu-icon-cut:before {
  content: "EA03";
}

.context-menu-icon-delete:before {
  content: "EA04";
}

.context-menu-icon-edit:before {
  content: "EA05";
}

.context-menu-icon-loading:before {
  content: "EA06";
}

.context-menu-icon-paste:before {
  content: "EA07";
}

.context-menu-icon-quit:before {
  content: "EA08";
}

.context-menu-icon::before {
  position: absolute;
  top: 50%;
  left: 0;
  width: 2em;
  font-family: "context-menu-icons";
  font-size: 1em;
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  color: #2980b9;
  text-align: center;
  -webkit-transform: translateY(-50%);
      -ms-transform: translateY(-50%);
       -o-transform: translateY(-50%);
          transform: translateY(-50%);

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.context-menu-icon.context-menu-hover:before {
  color: #fff;
}

.context-menu-icon.context-menu-disabled::before {
  color: #bbb;
}

.context-menu-icon.context-menu-icon-loading:before {
  -webkit-animation: cm-spin 2s infinite;
       -o-animation: cm-spin 2s infinite;
          animation: cm-spin 2s infinite;
}

.context-menu-icon.context-menu-icon--fa {
  display: list-item;
  font-family: inherit;
}
.context-menu-icon.context-menu-icon--fa::before {
  position: absolute;
  top: 50%;
  left: 0;
  width: 2em;
  font-family: FontAwesome;
  font-size: 1em;
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  color: #2980b9;
  text-align: center;
  -webkit-transform: translateY(-50%);
      -ms-transform: translateY(-50%);
       -o-transform: translateY(-50%);
          transform: translateY(-50%);

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.context-menu-icon.context-menu-icon--fa.context-menu-hover:before {
  color: #fff;
}
.context-menu-icon.context-menu-icon--fa.context-menu-disabled::before {
  color: #bbb;
}

.context-menu-list {
  position: absolute;
  display: inline-block;
  min-width: 13em;
  max-width: 26em;
  padding: .25em 0;
  margin: .3em;
  font-family: inherit;
  font-size: inherit;
  list-style-type: none;
  background: #fff;
  border: 1px solid #bebebe;
  border-radius: .2em;
  -webkit-box-shadow: 0 2px 5px rgba(0, 0, 0, .5);
          box-shadow: 0 2px 5px rgba(0, 0, 0, .5);
}

.context-menu-item {
  position: relative;
  padding: .2em 2em;
  color: #2f2f2f;
  -webkit-user-select: none;
     -moz-user-select: none;
      -ms-user-select: none;
          user-select: none;
  background-color: #fff;
}

.context-menu-separator {
  padding: 0;
  margin: .35em 0;
  border-bottom: 1px solid #e6e6e6;
}

.context-menu-item > label > input,
.context-menu-item > label > textarea {
  -webkit-user-select: text;
     -moz-user-select: text;
      -ms-user-select: text;
          user-select: text;
}

.context-menu-item.context-menu-hover {
  color: #fff;
  cursor: pointer;
  background-color: #2980b9;
}

.context-menu-item.context-menu-disabled {
  color: #bbb;
  cursor: default;
  background-color: #fff;
}

.context-menu-input.context-menu-hover {
  color: #2f2f2f;
  cursor: default;
}

.context-menu-submenu:after {
  position: absolute;
  top: 50%;
  right: .5em;
  z-index: 1;
  width: 0;
  height: 0;
  content: '';
  border-color: transparent transparent transparent #2f2f2f;
  border-style: solid;
  border-width: .25em 0 .25em .25em;
  -webkit-transform: translateY(-50%);
      -ms-transform: translateY(-50%);
       -o-transform: translateY(-50%);
          transform: translateY(-50%);
}

/**
 * Inputs
 */
.context-menu-item.context-menu-input {
  padding: .3em .6em;
}

/* vertically align inside labels */
.context-menu-input > label > * {
  vertical-align: top;
}

/* position checkboxes and radios as icons */
.context-menu-input > label > input[type="checkbox"],
.context-menu-input > label > input[type="radio"] {
  position: relative;
  top: .12em;
  margin-right: .4em;
}

.context-menu-input > label {
  margin: 0;
}

.context-menu-input > label,
.context-menu-input > label > input[type="text"],
.context-menu-input > label > textarea,
.context-menu-input > label > select {
  display: block;
  width: 100%;
  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
}

.context-menu-input > label > textarea {
  height: 7em;
}

.context-menu-item > .context-menu-list {
  top: .3em;
  /* re-positioned by js */
  right: -.3em;
  display: none;
}

.context-menu-item.context-menu-visible > .context-menu-list {
  display: block;
}

.context-menu-accesskey {
  text-decoration: underline;
}
</style><style type="text/css">
@import url('https://fonts.googleapis.com/css?family=Lato');

.context-menu-list {
  font-family: 'Lato', sans-serif !important;
  font-size: 14px;
  text-align: left;
  font-weight: normal;
  width: 200px;
}
.context-menu-item {
  font-weight: inherit;
  font-size: inherit;
  line-height: inherit;
  text-align: left;
}
.contextmenu-item-custom.contextmenu-item-custom__accent:not(:hover) {
  background-color: #f8ffeb;
}
.contextmenu-item-custom.contextmenu-item-custom__success:not(:hover) {
  background-color: #eeffcd;
}
</style></head>


  <body class="d-lg-flex">
    <!-- product > category > maptopic > article -->
<div class="sidebar d-none d-lg-block">

  <div class="d-flex flex-items-center p-4 position-sticky top-0 sidebar-background-color" style="z-index: 3;" id="github-logo" role="banner">
    <a href="/en" class="text-white" aria-hidden="true" tabindex="-1">
      <svg version="1.1" width="32" height="32" viewBox="0 0 16 16" class="octicon octicon-mark-github" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
    </a>
    <a href="/en" class="h4-mktg text-white no-underline no-wrap pl-2 flex-auto">GitHub Docs</a>
  </div>

  <nav>
    
    <ul class="sidebar-products">
      <!--
  Styling note:

  Categories, Maptopics, and Articles list items get a class of `active` when they correspond to content
  hierarchy of the current page. If an item's URL is also the same as the current URL, the item
  also gets an `is-current-page` class.
 -->



<li title="Home">
  <a href="/en" class="f6 pl-4 pr-5 ml-n1 pb-1">
    <svg xmlns="http://www.w3.org/2000/svg" class="octicon" viewBox="0 0 16 16" width="16" height="16">  <path fill-rule="evenodd" clip-rule="evenodd" d="M7.78033 12.5303C7.48744 12.8232 7.01256 12.8232 6.71967 12.5303L2.46967 8.28033C2.17678 7.98744 2.17678 7.51256 2.46967 7.21967L6.71967 2.96967C7.01256 2.67678 7.48744 2.67678 7.78033 2.96967C8.07322 3.26256 8.07322 3.73744 7.78033 4.03033L4.81066 7L12.25 7C12.6642 7 13 7.33579 13 7.75C13 8.16421 12.6642 8.5 12.25 8.5L4.81066 8.5L7.78033 11.4697C8.07322 11.7626 8.07322 12.2374 7.78033 12.5303Z"></path></svg>
    All products
  </a>
</li>


<li title="GitHub.com" class="sidebar-product mb-2">
  
  <a href="/en/github" class="pl-4 pr-5 pb-1 f4">GitHub.com</a>
  
</li>
<li>
<ul class="sidebar-categories list-style-none">
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/getting-started-with-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Getting started</a>
          
          
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
      
      <ul class="sidebar-topics list-style-none position-relative">
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/getting-started-with-github/quickstart" class="pl-4 pr-5 py-2">Quickstart</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/set-up-git" class="pl-6 pr-5 py-1">Set up Git</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/create-a-repo" class="pl-6 pr-5 py-1">Create a repo</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/fork-a-repo" class="pl-6 pr-5 py-1">Fork a repo</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/be-social" class="pl-6 pr-5 py-1">Be social</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/github-glossary" class="pl-6 pr-5 py-1">GitHub glossary</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/git-cheatsheet" class="pl-6 pr-5 py-1">Git cheatsheet</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/git-and-github-learning-resources" class="pl-6 pr-5 py-1 pb-2">Git and GitHub learning resources</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/getting-started-with-github/learning-about-github" class="pl-4 pr-5 py-2">Learning about GitHub</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/githubs-products" class="pl-6 pr-5 py-1">GitHub's products</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/about-github-advanced-security" class="pl-6 pr-5 py-1">About GitHub Advanced Security</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/types-of-github-accounts" class="pl-6 pr-5 py-1">Types of GitHub accounts</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/access-permissions-on-github" class="pl-6 pr-5 py-1">Access permissions on GitHub</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/faq-about-changes-to-githubs-plans" class="pl-6 pr-5 py-1 pb-2">FAQ about changes to GitHub’s plans</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/getting-started-with-github/signing-up-for-github" class="pl-4 pr-5 py-2">Signing up for GitHub</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/signing-up-for-a-new-github-account" class="pl-6 pr-5 py-1">Sign up for a new GitHub account</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/verifying-your-email-address" class="pl-6 pr-5 py-1">Verifying your email address</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/setting-up-a-trial-of-github-enterprise-cloud" class="pl-6 pr-5 py-1">Setting up a trial of GitHub Enterprise Cloud</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/setting-up-a-trial-of-github-enterprise-server" class="pl-6 pr-5 py-1 pb-2">Setting up a trial of GitHub Enterprise Server</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/getting-started-with-github/using-github" class="pl-4 pr-5 py-2">Using GitHub</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/exploring-early-access-releases-with-feature-preview" class="pl-6 pr-5 py-1">Exploring early access releases with feature preview</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/supported-browsers" class="pl-6 pr-5 py-1">Supported browsers</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/github-cli" class="pl-6 pr-5 py-1">GitHub CLI</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/github-desktop" class="pl-6 pr-5 py-1">GitHub Desktop</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/github-for-mobile" class="pl-6 pr-5 py-1">GitHub for mobile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/keyboard-shortcuts" class="pl-6 pr-5 py-1">Keyboard shortcuts</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/troubleshooting-connectivity-problems" class="pl-6 pr-5 py-1 pb-2">Troubleshooting connectivity problems</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/getting-started-with-github/exploring-projects-on-github" class="pl-4 pr-5 py-2">Exploring projects on GitHub</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/finding-ways-to-contribute-to-open-source-on-github" class="pl-6 pr-5 py-1">Finding ways to contribute to open source on GitHub</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/saving-repositories-with-stars" class="pl-6 pr-5 py-1">Saving repositories with stars</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/getting-started-with-github/following-people" class="pl-6 pr-5 py-1 pb-2">Following people</a>
                </li>
                
                
              </ul>
            </li>
          
        
      </ul>
      <!-- some categories have no maptopics, only articles -->
      
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/setting-up-and-managing-your-github-user-account" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">User accounts</a>
          
          
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
      
      <ul class="sidebar-topics list-style-none position-relative">
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-user-account-settings" class="pl-4 pr-5 py-2">Managing user account settings</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/about-your-personal-dashboard" class="pl-6 pr-5 py-1">About your personal dashboard</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-your-theme-settings" class="pl-6 pr-5 py-1">Managing your theme settings</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/changing-your-github-username" class="pl-6 pr-5 py-1">Changing your GitHub username</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/merging-multiple-user-accounts" class="pl-6 pr-5 py-1">Merging multiple user accounts</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/converting-a-user-into-an-organization" class="pl-6 pr-5 py-1">Converting a user into an organization</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/deleting-your-user-account" class="pl-6 pr-5 py-1">Deleting your user account</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-a-user-account-repository" class="pl-6 pr-5 py-1">Permission levels for a user account repository</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-user-owned-project-boards" class="pl-6 pr-5 py-1">Permission levels for user-owned project boards</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-the-default-branch-name-for-your-repositories" class="pl-6 pr-5 py-1">Managing the default branch name for your repositories</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-security-and-analysis-settings-for-your-user-account" class="pl-6 pr-5 py-1">Managing security and analysis settings for your user account</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-access-to-your-user-accounts-project-boards" class="pl-6 pr-5 py-1">Managing access to your user account's project boards</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/best-practices-for-leaving-your-company" class="pl-6 pr-5 py-1">Best practices for leaving your company</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/what-does-the-available-for-hire-checkbox-do" class="pl-6 pr-5 py-1 pb-2">What does the 'Available for hire' checkbox do?</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-email-preferences" class="pl-4 pr-5 py-2">Managing email preferences</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/adding-an-email-address-to-your-github-account" class="pl-6 pr-5 py-1">Adding an email address to your GitHub account</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/changing-your-primary-email-address" class="pl-6 pr-5 py-1">Changing your primary email address</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/setting-a-backup-email-address" class="pl-6 pr-5 py-1">Setting a backup email address</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/setting-your-commit-email-address" class="pl-6 pr-5 py-1">Setting your commit email address</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/blocking-command-line-pushes-that-expose-your-personal-email-address" class="pl-6 pr-5 py-1">Blocking command line pushes that expose your personal email address</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/remembering-your-github-username-or-email" class="pl-6 pr-5 py-1">Remembering your GitHub username or email</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/types-of-emails-github-sends" class="pl-6 pr-5 py-1">Types of emails GitHub sends</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-marketing-emails-from-github" class="pl-6 pr-5 py-1 pb-2">Managing marketing emails from GitHub</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories" class="pl-4 pr-5 py-2">Managing access to your personal repositories</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository" class="pl-6 pr-5 py-1">Inviting collaborators to a personal repository</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/removing-a-collaborator-from-a-personal-repository" class="pl-6 pr-5 py-1">Removing a collaborator from a personal repository</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/removing-yourself-from-a-collaborators-repository" class="pl-6 pr-5 py-1">Removing yourself from a collaborator's repository</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/maintaining-ownership-continuity-of-your-user-accounts-repositories" class="pl-6 pr-5 py-1 pb-2">Maintaining ownership continuity of your user account's repositories</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-your-membership-in-organizations" class="pl-4 pr-5 py-2">Managing your membership in organizations</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/about-organization-membership" class="pl-6 pr-5 py-1">About organization membership</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/accessing-an-organization" class="pl-6 pr-5 py-1">Accessing an organization</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/viewing-peoples-roles-in-an-organization" class="pl-6 pr-5 py-1">Viewing people's roles in an organization</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/requesting-organization-approval-for-oauth-apps" class="pl-6 pr-5 py-1">Requesting organization approval for OAuth Apps</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/publicizing-or-hiding-organization-membership" class="pl-6 pr-5 py-1">Publicizing or hiding organization membership</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/managing-your-scheduled-reminders" class="pl-6 pr-5 py-1">Managing your scheduled reminders</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-user-account/removing-yourself-from-an-organization" class="pl-6 pr-5 py-1 pb-2">Removing yourself from an organization</a>
                </li>
                
                
              </ul>
            </li>
          
        
      </ul>
      <!-- some categories have no maptopics, only articles -->
      
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/setting-up-and-managing-your-github-profile" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Profiles</a>
          
          
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
      
      <ul class="sidebar-topics list-style-none position-relative">
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/setting-up-and-managing-your-github-profile/customizing-your-profile" class="pl-4 pr-5 py-2">Customizing your profile</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/about-your-profile" class="pl-6 pr-5 py-1">About your profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/about-your-organizations-profile" class="pl-6 pr-5 py-1">About your organization's profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/personalizing-your-profile" class="pl-6 pr-5 py-1">Personalizing your profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/managing-your-profile-readme" class="pl-6 pr-5 py-1">Managing your profile README</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/pinning-items-to-your-profile" class="pl-6 pr-5 py-1 pb-2">Pinning items to your profile</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile" class="pl-4 pr-5 py-2">Managing contribution graphs on your profile</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/viewing-contributions-on-your-profile" class="pl-6 pr-5 py-1">Viewing contributions on your profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/showing-an-overview-of-your-activity-on-your-profile" class="pl-6 pr-5 py-1">Showing an overview of your activity on your profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/publicizing-or-hiding-your-private-contributions-on-your-profile" class="pl-6 pr-5 py-1">Publicizing or hiding your private contributions on your profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/sending-your-github-enterprise-server-contributions-to-your-githubcom-profile" class="pl-6 pr-5 py-1">Sending your GitHub Enterprise Server contributions to your GitHub.com profile</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/why-are-my-contributions-not-showing-up-on-my-profile" class="pl-6 pr-5 py-1">Why are my contributions not showing up on my profile?</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/setting-up-and-managing-your-github-profile/troubleshooting-commits-on-your-timeline" class="pl-6 pr-5 py-1 pb-2">Troubleshooting commits on your timeline</a>
                </li>
                
                
              </ul>
            </li>
          
        
      </ul>
      <!-- some categories have no maptopics, only articles -->
      
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/authenticating-to-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Authentication</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/managing-subscriptions-and-notifications-on-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Managing subscriptions and notifications on GitHub</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/setting-up-and-managing-organizations-and-teams" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Organizations and teams</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/setting-up-and-managing-your-enterprise" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Your enterprise</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/setting-up-and-managing-billing-and-payments-on-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Billing and payments</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/writing-on-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Writing on GitHub</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/creating-cloning-and-archiving-repositories" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Creating, cloning, and archiving repositories</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/using-git" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Using Git</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/committing-changes-to-your-project" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Committing changes to your project</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/collaborating-with-issues-and-pull-requests" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Collaborating with issues and pull requests</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/managing-your-work-on-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Managing your work on GitHub</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/developing-online-with-codespaces" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Codespaces</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/building-a-strong-community" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Building a strong community</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/searching-for-information-on-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Searching for information on GitHub</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/importing-your-projects-to-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Importing your projects</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/administering-a-repository" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Administering a repository</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/visualizing-repository-data-with-graphs" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Visualizing repository data with graphs</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/managing-security-vulnerabilities" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Supply chain security</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/finding-security-vulnerabilities-and-errors-in-your-code" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Secure coding</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/managing-files-in-a-repository" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Managing files in a repository</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/managing-large-files" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Managing large files</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/customizing-your-github-workflow" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Customizing your GitHub workflow</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/extending-github" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Extending GitHub</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 active ">
    
    <details class="dropdown-withArrow details details-reset" open="">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/working-with-github-pages" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">GitHub Pages</a>
          
          <svg xmlns="http://www.w3.org/2000/svg" class="octicon flex-shrink-0 arrow mr-3" style="margin-top:7px" viewBox="0 0 16 16" width="16" height="16"> <path fill-rule="evenodd" clip-rule="evenodd" d="M12.7803 6.21967C13.0732 6.51256 13.0732 6.98744 12.7803 7.28033L8.53033 11.5303C8.23744 11.8232 7.76256 11.8232 7.46967 11.5303L3.21967 7.28033C2.92678 6.98744 2.92678 6.51256 3.21967 6.21967C3.51256 5.92678 3.98744 5.92678 4.28033 6.21967L8 9.93934L11.7197 6.21967C12.0126 5.92678 12.4874 5.92678 12.7803 6.21967Z"></path></svg>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
      
      <ul class="sidebar-topics list-style-none position-relative">
        
          
            

            <li class="sidebar-maptopic active ">
              <a href="/en/github/working-with-github-pages/getting-started-with-github-pages" class="pl-4 pr-5 py-2">Getting started with GitHub Pages</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/about-github-pages" class="pl-6 pr-5 py-1">About GitHub Pages</a>
                </li>
                
                
                
                

                <li class="sidebar-article active is-current-page">
                  <a href="/en/github/working-with-github-pages/creating-a-github-pages-site" class="pl-6 pr-5 py-1">Creating a GitHub Pages site</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-with-the-theme-chooser" class="pl-6 pr-5 py-1">Adding a theme to your GitHub Pages site with the theme chooser</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site" class="pl-6 pr-5 py-1">Configuring a publishing source for your GitHub Pages site</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/changing-the-visibility-of-your-github-pages-site" class="pl-6 pr-5 py-1">Changing the visibility of your GitHub Pages site</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/creating-a-custom-404-page-for-your-github-pages-site" class="pl-6 pr-5 py-1">Creating a custom 404 page for your GitHub Pages site</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/securing-your-github-pages-site-with-https" class="pl-6 pr-5 py-1">Securing your GitHub Pages site with HTTPS</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/using-submodules-with-github-pages" class="pl-6 pr-5 py-1">Using submodules with GitHub Pages</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/unpublishing-a-github-pages-site" class="pl-6 pr-5 py-1 pb-2">Unpublishing a GitHub Pages site</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/working-with-github-pages/setting-up-a-github-pages-site-with-jekyll" class="pl-4 pr-5 py-2">Setting up a GitHub Pages site with Jekyll</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/about-github-pages-and-jekyll" class="pl-6 pr-5 py-1">About GitHub Pages and Jekyll</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll" class="pl-6 pr-5 py-1">Creating a GitHub Pages site with Jekyll</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll" class="pl-6 pr-5 py-1">Testing your GitHub Pages site locally with Jekyll</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/adding-content-to-your-github-pages-site-using-jekyll" class="pl-6 pr-5 py-1">Adding content to your GitHub Pages site using Jekyll</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/setting-a-markdown-processor-for-your-github-pages-site-using-jekyll" class="pl-6 pr-5 py-1">Setting a Markdown processor for your GitHub Pages site using Jekyll</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-using-jekyll" class="pl-6 pr-5 py-1">Adding a theme to your GitHub Pages site using Jekyll</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/about-jekyll-build-errors-for-github-pages-sites" class="pl-6 pr-5 py-1">About Jekyll build errors for GitHub Pages sites</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/troubleshooting-jekyll-build-errors-for-github-pages-sites" class="pl-6 pr-5 py-1 pb-2">Troubleshooting Jekyll build errors for GitHub Pages sites</a>
                </li>
                
                
              </ul>
            </li>
          
        
          
            

            <li class="sidebar-maptopic ">
              <a href="/en/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site" class="pl-4 pr-5 py-2">Configuring a custom domain for your GitHub Pages site</a>
              <ul class="sidebar-articles my-2">
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/about-custom-domains-and-github-pages" class="pl-6 pr-5 py-1">About custom domains and GitHub Pages</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/managing-a-custom-domain-for-your-github-pages-site" class="pl-6 pr-5 py-1">Managing a custom domain for your GitHub Pages site</a>
                </li>
                
                
                
                

                <li class="sidebar-article ">
                  <a href="/en/github/working-with-github-pages/troubleshooting-custom-domains-and-github-pages" class="pl-6 pr-5 py-1 pb-2">Troubleshooting custom domains and GitHub Pages</a>
                </li>
                
                
              </ul>
            </li>
          
        
      </ul>
      <!-- some categories have no maptopics, only articles -->
      
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/supporting-the-open-source-community-with-github-sponsors" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">GitHub Sponsors</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/finding-talent-with-github-jobs" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Finding talent with GitHub Jobs</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/working-with-github-support" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Working with GitHub Support</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/understanding-how-github-uses-and-protects-your-data" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Understanding how GitHub uses and protects your data</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
  

  <li class="sidebar-category py-1 ">
    
    <details class="dropdown-withArrow details details-reset">
      <summary>
        <div class="d-flex flex-justify-between">
          <a href="/en/github/site-policy" class="pl-4 pr-2 py-2 f6 text-uppercase d-block flex-auto mr-3">Site policy</a>
          
        </div>
      </summary>
    
      <!-- some categories have maptopics with child articles -->
      
    </details>
  </li>
  
</ul>
</li>

    </ul>
    
  </nav>
</div>


    <main class="width-full">
      <div class="border-bottom border-gray-light no-print">
  
  <!-- START TRANSLATIONS NOTICES -->

<!-- END TRANSLATIONS NOTICES -->

<!-- START RELEASE NOTICES -->
<!-- Custom GitHub AE notice -->

<!-- END RELEASE NOTICES -->

<!-- ONEOFF EARLY ACCESS NOTICE -->

<!-- END ONEOFF EARLY ACCESS NOTICE -->






  

  <header class="container-xl px-3 px-md-6 pt-3 pb-2 position-relative d-flex flex-justify-between width-full ">

    <div class="d-flex flex-items-center d-lg-none" style="z-index: 3;" id="github-logo-mobile" role="banner">
      <a href="/en" aria-hidden="true" tabindex="-1">
        <svg version="1.1" width="32" height="32" viewBox="0 0 16 16" class="octicon octicon-mark-github text-black" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
      </a>
      <a href="/en" class="h4-mktg text-gray-dark no-underline no-wrap pl-2">GitHub Docs</a>
    </div>

    <div class="width-full">
      <div class="d-inline-block width-full d-md-flex" style="z-index: 1;">
        <button class="nav-mobile-burgerIcon float-right mt-1 border-0 d-md-none" type="button" aria-label="Toggle navigation">
          <!-- Hamburger icon added with css -->
        </button>
        <div style="z-index: 2;" class="nav-mobile-dropdown width-full">
          <div class="d-md-flex flex-justify-between flex-items-center">
            <div class="py-2 py-md-0 d-md-inline-block">
              <h4 class="text-mono f5 text-normal text-gray d-md-none">Explore by product</h4>
              <details class="dropdown-withArrow position-relative details details-reset d-md-none close-when-clicked-outside">
                <summary class="nav-desktop-productDropdownButton text-blue-mktg py-2" role="button" aria-label="Toggle products list">
                  <div id="current-product" class="d-flex flex-items-center flex-justify-between" style="padding-top: 2px;">
                    <!-- Product switcher - GitHub.com, Enterprise Server, etc -->
                    <!-- 404 and 500 error layouts are not real pages so we need to hardcode the name for those -->
                    GitHub.com
                    <svg class="arrow ml-md-1" width="14px" height="8px" viewBox="0 0 14 8" xml:space="preserve" fill="none" stroke="#1277eb"><path d="M1,1l6.2,6L13,1"></path></svg>
                  </div>
                </summary>
                <!-- Mobile-only product dropdown -->
                <div id="homepages" class="position-md-absolute nav-desktop-productDropdown p-md-4 left-md-n4 top-md-6" style="z-index: 6;">
                  
                  <a href="/en/github" class="d-block py-2
                      text-blue-mktg text-underline active">
                      GitHub.com
                      
                  </a>
                  
                  <a href="/en/enterprise-server@3.0/admin" class="d-block py-2
                      link-gray-dark no-underline">
                      Enterprise Administrators
                      
                  </a>
                  
                  <a href="/en/discussions" class="d-block py-2
                      link-gray-dark no-underline">
                      GitHub Discussions
                      
                  </a>
                  
                  <a href="/en/code-security" class="d-block py-2
                      link-gray-dark no-underline">
                      Code security
                      
                  </a>
                  
                  <a href="/en/actions" class="d-block py-2
                      link-gray-dark no-underline">
                      GitHub Actions
                      
                  </a>
                  
                  <a href="/en/packages" class="d-block py-2
                      link-gray-dark no-underline">
                      GitHub Packages
                      
                  </a>
                  
                  <a href="/en/developers" class="d-block py-2
                      link-gray-dark no-underline">
                      Developers
                      
                  </a>
                  
                  <a href="/en/rest" class="d-block py-2
                      link-gray-dark no-underline">
                      REST API
                      
                  </a>
                  
                  <a href="/en/graphql" class="d-block py-2
                      link-gray-dark no-underline">
                      GraphQL API
                      
                  </a>
                  
                  <a href="/en/enterprise-server@3.0/insights" class="d-block py-2
                      link-gray-dark no-underline">
                      GitHub Insights
                      
                  </a>
                  
                  <a href="/en/education" class="d-block py-2
                      link-gray-dark no-underline">
                      Education
                      
                  </a>
                  
                  <a href="/en/desktop" class="d-block py-2
                      link-gray-dark no-underline">
                      GitHub Desktop
                      
                  </a>
                  
                  <a href="https://cli.github.com/manual" class="d-block py-2
                      link-gray-dark no-underline">
                      GitHub CLI
                      
                      <span class="ml-1"><svg width="9" height="10" viewBox="0 0 9 10" fill="none" xmlns="http://www.w3.org/2000/svg"><path stroke="#24292e" d="M.646 8.789l8-8M8.5 9V1M1 .643h8"></path></svg></span>
                      
                  </a>
                  
                  <a href="https://atom.io/docs" class="d-block py-2
                      link-gray-dark no-underline">
                      Atom
                      
                      <span class="ml-1"><svg width="9" height="10" viewBox="0 0 9 10" fill="none" xmlns="http://www.w3.org/2000/svg"><path stroke="#24292e" d="M.646 8.789l8-8M8.5 9V1M1 .643h8"></path></svg></span>
                      
                  </a>
                  
                  <a href="https://electronjs.org/docs" class="d-block py-2
                      link-gray-dark no-underline">
                      Electron
                      
                      <span class="ml-1"><svg width="9" height="10" viewBox="0 0 9 10" fill="none" xmlns="http://www.w3.org/2000/svg"><path stroke="#24292e" d="M.646 8.789l8-8M8.5 9V1M1 .643h8"></path></svg></span>
                      
                  </a>
                  
                </div>
              </details>
            </div>

            <!-- Versions picker that only appears in the header on homepage/versioned homepages -->
            <!-- Versions picker that only appears in the header on homepage/versioned homepages -->



            <div class="d-md-inline-block">

              <!-- Language picker - 'English', 'Japanese', etc -->
              
                <div class="border-top border-md-top-0 py-2 py-md-0 d-md-inline-block">
                  <details class="dropdown-withArrow position-relative details details-reset mr-md-3 close-when-clicked-outside">
                    <summary class="py-2 text-gray-dark" role="button" aria-label="Toggle languages list">
                      <div class="d-flex flex-items-center flex-justify-between">
                        
                          English
                        
                        <svg class="arrow ml-md-1" width="14px" height="8px" viewBox="0 0 14 8" xml:space="preserve" fill="none" stroke="#1B1F23"><path d="M1,1l6.2,6L13,1"></path></svg>
                      </div>
                    </summary>
                    <div id="languages-selector" class="position-md-absolute nav-desktop-langDropdown p-md-4 right-md-n4 top-md-6" style="z-index: 6;">
                    
                      
                        <a href="/en/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 no-underline active link-gray" style="white-space: nowrap">
                          
                            English
                          
                        </a>
                      
                    
                      
                        <a href="/cn/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 no-underline link-gray-dark" style="white-space: nowrap">
                          
                            简体中文 (Simplified Chinese)
                          
                        </a>
                      
                    
                      
                        <a href="/ja/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 no-underline link-gray-dark" style="white-space: nowrap">
                          
                            日本語 (Japanese)
                          
                        </a>
                      
                    
                      
                        <a href="/es/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 no-underline link-gray-dark" style="white-space: nowrap">
                          
                            Español (Spanish)
                          
                        </a>
                      
                    
                      
                        <a href="/pt/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 no-underline link-gray-dark" style="white-space: nowrap">
                          
                            Português do Brasil (Portuguese)
                          
                        </a>
                      
                    
                      
                    
                    </div>
                  </details>
                </div>
              

              <!-- GitHub.com homepage and 404 page has a stylized search; Enterprise homepages do not -->
              
              <div class="pt-3 pt-md-0 d-md-inline-block ml-md-3 border-top border-md-top-0">
                <!--
  This form is used in two places:

  - On the homepage, front and center
  - On all other pages, in the header
 -->

<div id="search-input-container" aria-hidden="true">
  <!-- will add a search input here -->
<div class="ais-SearchBox"><form role="search" class="ais-SearchBox-form" novalidate="true"><input class="ais-SearchBox-input" type="search" placeholder="Search topics, products..." autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false" maxlength="512"><button class="ais-SearchBox-submit" type="submit" title="Submit the search query." hidden="true"></button></form></div></div>

                <div id="search-results-container"></div>
                <div class="search-overlay-desktop"></div>
              </div>
              

            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</div>

      

      
        <div class="container-xl px-3 px-md-6 my-4 my-lg-4 d-xl-flex">
  <article class="markdown-body width-full">
    <div class="d-lg-flex flex-justify-between">
      <div class="d-block d-lg-none">
  <details class="dropdown-withArrow d-inline-block details details-reset mb-1 position-relative close-when-clicked-outside article-versions">
    <summary class="f4 h5-mktg btn-outline-mktg btn-mktg p-2">
      <!-- GitHub.com, Enterprise Server 2.16, etc -->
      <span class="d-md-none d-xl-inline-block">Article version:</span> GitHub.com
      <svg class="arrow ml-1" width="14px" height="8px" viewBox="0 0 14 8" xml:space="preserve" fill="none" stroke="#1277eb"><path d="M1,1l6.2,6L13,1"></path></svg>
    </summary>

    <div class="nav-dropdown position-absolute bg-white rounded-1 px-4 py-3 top-7 box-shadow-large" style="z-index: 6; width: 210px;">
      
      <a href="/en/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-blue active">
      GitHub.com</a>
      
      <a href="/en/enterprise-server@3.0/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      Enterprise Server 3.0</a>
      
      <a href="/en/enterprise-server@2.22/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      Enterprise Server 2.22</a>
      
      <a href="/en/enterprise-server@2.21/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      Enterprise Server 2.21</a>
      
      <a href="/en/github-ae@latest/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      GitHub AE</a>
      
      <a class="f6 no-underline text-gray-light pt-1" href="/enterprise-server-releases">See all Enterprise releases</a>
    </div>
  </details>

</div>
      <div class="d-flex flex-items-center breadcrumbs-wrapper">
        <nav class="breadcrumbs f5" aria-label="Breadcrumb">
  
    
      <a title="product: GitHub.com" href="/en/github" class="d-inline-block ">
        GitHub.com
      </a>
    
  
    
      <a title="category: GitHub Pages" href="/en/github/working-with-github-pages" class="d-inline-block ">
        GitHub Pages
      </a>
    
  
    
      <a title="maptopic: Getting started with GitHub Pages" href="/en/github/working-with-github-pages/getting-started-with-github-pages" class="d-inline-block ">
        Getting started with GitHub Pages
      </a>
    
  
    
      <a title="article: Creating a GitHub Pages site" href="/en/github/working-with-github-pages/creating-a-github-pages-site" class="d-inline-block text-gray-light">
        Creating a GitHub Pages site
      </a>
    
  
</nav>

      </div>
      <div class="d-none d-lg-block">
  <details class="dropdown-withArrow d-inline-block details details-reset mb-1 position-relative close-when-clicked-outside article-versions">
    <summary class="f4 h5-mktg btn-outline-mktg btn-mktg p-2">
      <!-- GitHub.com, Enterprise Server 2.16, etc -->
      <span class="d-md-none d-xl-inline-block">Article version:</span> GitHub.com
      <svg class="arrow ml-1" width="14px" height="8px" viewBox="0 0 14 8" xml:space="preserve" fill="none" stroke="#1277eb"><path d="M1,1l6.2,6L13,1"></path></svg>
    </summary>

    <div class="nav-dropdown position-absolute bg-white rounded-1 px-4 py-3 top-7 box-shadow-large" style="z-index: 6; width: 210px;">
      
      <a href="/en/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-blue active">
      GitHub.com</a>
      
      <a href="/en/enterprise-server@3.0/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      Enterprise Server 3.0</a>
      
      <a href="/en/enterprise-server@2.22/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      Enterprise Server 2.22</a>
      
      <a href="/en/enterprise-server@2.21/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      Enterprise Server 2.21</a>
      
      <a href="/en/github-ae@latest/github/working-with-github-pages/creating-a-github-pages-site" class="d-block py-2 link-gray-dark no-underline">
      GitHub AE</a>
      
      <a class="f6 no-underline text-gray-light pt-1" href="/enterprise-server-releases">See all Enterprise releases</a>
    </div>
  </details>

</div>
    </div>

    <div class="mt-2 article-grid-container">

    <div class="article-grid-head">
      <div class="d-flex flex-items-baseline flex-justify-between mt-3">
        <h1 class="border-bottom-0">Creating a GitHub Pages site</h1>
        <div class="d-none d-lg-block ml-2">
          <button class="btn-link link-gray js-print tooltipped tooltipped-n" aria-label="Print this article">
            <!-- From https://heroicons.dev/ -->
<svg fill="none" height="18" width="18" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M17 17h2a2 2 0 002-2v-4a2 2 0 00-2-2H5a2 2 0 00-2 2v4a2 2 0 002 2h2m2 4h6a2 2 0 002-2v-4a2 2 0 00-2-2H9a2 2 0 00-2 2v4a2 2 0 002 2zm8-12V5a2 2 0 00-2-2H9a2 2 0 00-2 2v4h10z"></path></svg>
          </button>
        </div>
      </div>

      

      
        <div class="lead-mktg"><p>You can create a GitHub Pages site in a new or existing repository.</p></div>
      

      

      

      
        <div class="product-callout border rounded-1 mb-4 p-3 border-purple bg-purple-light">
        <p>GitHub Pages is available in public repositories with GitHub Free and GitHub Free for organizations, and in public and private repositories with GitHub Pro, GitHub Team, GitHub Enterprise Cloud, and GitHub Enterprise Server. For more information, see "<a href="/en/articles/github-s-products">GitHub's products</a>."</p>
        </div>
      
    </div>
    <div class="article-grid-toc border-bottom border-xl-0 pb-4 mb-5 pb-xl-0 mb-xl-0">
      <div class="article-grid-toc-content">
        
        <h2 id="in-this-article" class="f5 mb-2"><a class="link-gray-dark" href="#in-this-article">In this article</a></h2>
        <ul class="list-style-none pl-0 f5 mb-0">
          
          <li class="ml-0  mb-2 lh-condensed"><a href="#creating-a-repository-for-your-site">Creating a repository for your site</a></li>
          
          <li class="ml-0  mb-2 lh-condensed"><a href="#creating-your-site">Creating your site</a></li>
          
          <li class="ml-0  mb-2 lh-condensed"><a href="#next-steps">Next steps</a></li>
          
          <li class="ml-0  mb-2 lh-condensed"><a href="#further-reading">Further reading</a></li>
          
        </ul>
        
      </div>
    </div>
    <div id="article-contents" class="article-grid-body">
      
      <div class="extended-markdown note border rounded-1 mb-4 p-3 border-blue bg-blue-light f5">
<p><strong>Note:</strong> Organization owners can restrict the publication of GitHub Pages sites from repositories owned by the organization. For more information, see "<a href="/en/github/setting-up-and-managing-organizations-and-teams/managing-the-publication-of-github-pages-sites-for-your-organization">Managing the publication of GitHub Pages sites</a>."</p>
</div>
<h3 id="creating-a-repository-for-your-site"><a href="#creating-a-repository-for-your-site">Creating a repository for your site</a></h3>
<p>If your site is an independent project, you can create a new repository to store your site's source code. If your site is associated with an existing project, you can add the source code to that project's repository, in a <code>/docs</code> folder on the default branch or on a different branch. For example, if you're creating a site to publish documentation for a project that's already on GitHub, you may want to store the source code for the site in the same repository as the project.</p>
<p>If the account that owns the repository uses GitHub Free or GitHub Free for organizations, the repository must be public.</p>
<p>If you want to create a site in an existing repository, skip to the "<a href="#creating-your-site">Creating your site</a>" section.</p>
<ol>
<li>In the upper-right corner of any page, use the <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-plus" aria-label="Plus symbol" role="img"><path fill-rule="evenodd" d="M8 2a.75.75 0 01.75.75v4.5h4.5a.75.75 0 010 1.5h-4.5v4.5a.75.75 0 01-1.5 0v-4.5h-4.5a.75.75 0 010-1.5h4.5v-4.5A.75.75 0 018 2z"></path></svg> drop-down menu, and select <strong>New repository</strong>.
<div><img src="/assets/images/help/repository/repo-create.png" alt="Drop-down with option to create a new repository"></div></li>
<li>Use the <strong>Owner</strong> drop-down menu, and select the account you want to own the repository.
<div><img src="/assets/images/help/repository/create-repository-owner.png" alt="Owner drop-down menu"></div></li>
<li>Type a name for your repository and an optional description. If you're creating a user or organization site, your repository must be named <code>&lt;user&gt;.github.io</code> or <code>&lt;organization&gt;.github.io</code>. For more information, see "<a href="/en/articles/about-github-pages#types-of-github-pages-sites">About GitHub Pages</a>."
<div><img src="/assets/images/help/pages/create-repository-name-pages.png" alt="Create repository field"></div></li>
<li>Choose a repository visibility. For more information, see "<a href="/en/github/creating-cloning-and-archiving-repositories/about-repository-visibility">About repository visibility</a>."
<div><img src="/assets/images/help/repository/create-repository-public-private.png" alt="Radio buttons to select repository visibility"></div></li>
<li>Select <strong>Initialize this repository with a README</strong>.
<div><img src="/assets/images/help/repository/initialize-with-readme.png" alt="Initialize this repository with a README checkbox"></div></li>
<li>Click <strong>Create repository</strong>.
<div><img src="/assets/images/help/repository/create-repository-button.png" alt="Button to create repository"></div></li>
</ol>
<h3 id="creating-your-site"><a href="#creating-your-site">Creating your site</a></h3>
<p>Before you can create your site, you must have a repository for your site on GitHub. If you're not creating your site in an existing repository, see "<a href="#creating-a-repository-for-your-site">Creating a repository for your site</a>."</p>
<div class="extended-markdown warning border rounded-1 mb-4 p-3 border-red bg-red-light f5">
<p><strong>Warning</strong>: GitHub Pages sites are publicly available on the internet by default, even if the repository for the site is private or internal. If your project site is published from a private or internal repository owned by an organization using GitHub Enterprise Cloud, you can manage access control for the site. Otherwise, if you have sensitive data in your site's repository, you may want to remove the data before publishing. For more information, see "<a href="/en/github/creating-cloning-and-archiving-repositories/about-repository-visibility">About repository visibility</a>" and "<a href="/en/github/working-with-github-pages/changing-the-visibility-of-your-github-pages-site">Changing the visibility of your GitHub Pages site</a>."</p>
</div>
<ol>
<li>
<p>On GitHub, navigate to your site's repository.</p>
</li>
<li>
<p>Decide which publishing source you want to use.  For more information, see "<a href="/en/articles/about-github-pages#publishing-sources-for-github-pages-sites">About GitHub Pages</a>."</p>
</li>
<li>
<p>If your chosen publishing source already exists, navigate to the publishing source. If your chosen publishing source doesn't exist, create the publishing source.</p>
</li>
<li>
<p>In the root of the publishing source, create a new file called <code>index.md</code> that contains the content you want to display on the main page of your site.</p>
</li>
<li>
<p>Configure your publishing source. For more information, see "<a href="/en/articles/configuring-a-publishing-source-for-your-github-pages-site#choosing-a-publishing-source">Configuring a publishing source for your GitHub Pages site</a>."</p>
</li>
<li>
<p>Under your repository name, click <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-gear" aria-label="The gear icon" role="img"><path fill-rule="evenodd" d="M7.429 1.525a6.593 6.593 0 011.142 0c.036.003.108.036.137.146l.289 1.105c.147.56.55.967.997 1.189.174.086.341.183.501.29.417.278.97.423 1.53.27l1.102-.303c.11-.03.175.016.195.046.219.31.41.641.573.989.014.031.022.11-.059.19l-.815.806c-.411.406-.562.957-.53 1.456a4.588 4.588 0 010 .582c-.032.499.119 1.05.53 1.456l.815.806c.08.08.073.159.059.19a6.494 6.494 0 01-.573.99c-.02.029-.086.074-.195.045l-1.103-.303c-.559-.153-1.112-.008-1.529.27-.16.107-.327.204-.5.29-.449.222-.851.628-.998 1.189l-.289 1.105c-.029.11-.101.143-.137.146a6.613 6.613 0 01-1.142 0c-.036-.003-.108-.037-.137-.146l-.289-1.105c-.147-.56-.55-.967-.997-1.189a4.502 4.502 0 01-.501-.29c-.417-.278-.97-.423-1.53-.27l-1.102.303c-.11.03-.175-.016-.195-.046a6.492 6.492 0 01-.573-.989c-.014-.031-.022-.11.059-.19l.815-.806c.411-.406.562-.957.53-1.456a4.587 4.587 0 010-.582c.032-.499-.119-1.05-.53-1.456l-.815-.806c-.08-.08-.073-.159-.059-.19a6.44 6.44 0 01.573-.99c.02-.029.086-.075.195-.045l1.103.303c.559.153 1.112.008 1.529-.27.16-.107.327-.204.5-.29.449-.222.851-.628.998-1.189l.289-1.105c.029-.11.101-.143.137-.146zM8 0c-.236 0-.47.01-.701.03-.743.065-1.29.615-1.458 1.261l-.29 1.106c-.017.066-.078.158-.211.224a5.994 5.994 0 00-.668.386c-.123.082-.233.09-.3.071L3.27 2.776c-.644-.177-1.392.02-1.82.63a7.977 7.977 0 00-.704 1.217c-.315.675-.111 1.422.363 1.891l.815.806c.05.048.098.147.088.294a6.084 6.084 0 000 .772c.01.147-.038.246-.088.294l-.815.806c-.474.469-.678 1.216-.363 1.891.2.428.436.835.704 1.218.428.609 1.176.806 1.82.63l1.103-.303c.066-.019.176-.011.299.071.213.143.436.272.668.386.133.066.194.158.212.224l.289 1.106c.169.646.715 1.196 1.458 1.26a8.094 8.094 0 001.402 0c.743-.064 1.29-.614 1.458-1.26l.29-1.106c.017-.066.078-.158.211-.224a5.98 5.98 0 00.668-.386c.123-.082.233-.09.3-.071l1.102.302c.644.177 1.392-.02 1.82-.63.268-.382.505-.789.704-1.217.315-.675.111-1.422-.364-1.891l-.814-.806c-.05-.048-.098-.147-.088-.294a6.1 6.1 0 000-.772c-.01-.147.039-.246.088-.294l.814-.806c.475-.469.679-1.216.364-1.891a7.992 7.992 0 00-.704-1.218c-.428-.609-1.176-.806-1.82-.63l-1.103.303c-.066.019-.176.011-.299-.071a5.991 5.991 0 00-.668-.386c-.133-.066-.194-.158-.212-.224L10.16 1.29C9.99.645 9.444.095 8.701.031A8.094 8.094 0 008 0zm1.5 8a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM11 8a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
<strong>Settings</strong>.
</p><div><img src="/assets/images/help/repository/repo-actions-settings.png" alt="Repository settings button"></div><p></p>
</li>
<li>
<p>Optionally, if you're publishing a project site from a private or internal repository owned by an organization using GitHub Enterprise Cloud, choose the visibility for your site. Under "GitHub Pages", select the <strong>GitHub Pages visibility</strong> drop-down menu, then click a visibility. For more information, see "<a href="/en/github/working-with-github-pages/changing-the-visibility-of-your-github-pages-site">Changing the visibility of your GitHub Pages site</a>".
</p><div><img src="/assets/images/help/pages/public-or-private-visibility.png" alt="Drop-down to select visibility for your site"></div><p></p>
</li>
<li>
<p>To see your published site, under "GitHub Pages", click your site's URL.
</p><div><img src="/assets/images/help/pages/click-pages-url-to-preview.png" alt="URL of your published site"></div><p></p>
  <div class="extended-markdown note border rounded-1 mb-4 p-3 border-blue bg-blue-light f5">
<p>  <strong>Note:</strong> It can take up to 20 minutes for changes to your site to publish after you push the changes to GitHub. If your don't see your changes reflected in your browser after an hour, see "<a href="/en/articles/about-jekyll-build-errors-for-github-pages-sites">About Jekyll build errors for GitHub Pages sites</a>."</p>
  </div>
</li>
</ol>
<div class="extended-markdown tip border rounded-1 mb-4 p-3 border-blue bg-blue-light f5">
<p><strong>Note</strong>: If your site has not published automatically, make sure someone with admin permissions and a verified email address has pushed to the publishing source.</p>
</div>
<h3 id="next-steps"><a href="#next-steps">Next steps</a></h3>
<p>You can add more pages to your site by creating more new files. Each file will be available on your site in the same directory structure as your publishing source. For example, if the publishing source for your project site is the <code>gh-pages</code> branch, and you create a new file called <code>/about/contact-us.md</code> on the <code>gh-pages</code> branch, the file will be available at <code>https://&lt;user&gt;.github.io/&lt;repository&gt;/about/contact-us.html</code>.</p>
<p>You can also add a theme to customize your site’s look and feel. For more information, see "<a href="/en/articles/adding-a-theme-to-your-github-pages-site-with-the-theme-chooser">Adding a theme to your GitHub Pages site with the theme chooser</a>."</p>
<p>To customize your site even more, you can use Jekyll, a static site generator with built-in support for GitHub Pages. For more information, see "<a href="/en/articles/about-github-pages-and-jekyll">About GitHub Pages and Jekyll</a>."</p>
<h3 id="further-reading"><a href="#further-reading">Further reading</a></h3>
<ul>
<li>"<a href="/en/articles/troubleshooting-jekyll-build-errors-for-github-pages-sites">Troubleshooting Jekyll build errors for GitHub Pages sites</a>"</li>
<li>"<a href="/en/articles/creating-and-deleting-branches-within-your-repository">Creating and deleting branches within your repository</a>"</li>
<li>"<a href="/en/articles/creating-new-files">Creating new files</a>"</li>
</ul>
    </div>
    </div>

    <div class="d-block mt-4 markdown-body">
      
    </div>
  </article>
</div>

      
      <section class="mt-lg-9 py-7 px-3 px-md-6 no-print" style="background:#fafbfc">
  <div class="container-xl gutter-lg-spacious clearfix">
    <div class="col-12 col-lg-6 col-xl-4 mb-6 mb-xl-0 float-left">
      
<form class="js-helpfulness f5">
  <h2 data-help-start="" data-help-yes="" data-help-no="" class="mb-1 f4">
    Did this doc help you?
  </h2>
  <p class="f6">
    <a href="/github/site-policy/github-privacy-statement">Privacy policy</a>
  </p>
  <p class="radio-group" data-help-start="" data-help-yes="" data-help-no="">
    <input hidden="" id="helpfulness-yes" type="radio" name="helpfulness-vote" value="Yes" aria-label="Yes">
    <label class="btn x-radio-label" for="helpfulness-yes">
      <svg version="1.1" width="24" height="24" viewBox="0 0 24 24" class="octicon octicon-thumbsup" aria-hidden="true"><path fill-rule="evenodd" d="M12.596 2.043c-1.301-.092-2.303.986-2.303 2.206v1.053c0 2.666-1.813 3.785-2.774 4.2a1.866 1.866 0 01-.523.131A1.75 1.75 0 005.25 8h-1.5A1.75 1.75 0 002 9.75v10.5c0 .967.784 1.75 1.75 1.75h1.5a1.75 1.75 0 001.742-1.58c.838.06 1.667.296 2.69.586l.602.17c1.464.406 3.213.824 5.544.824 2.188 0 3.693-.204 4.583-1.372.422-.554.65-1.255.816-2.05.148-.708.262-1.57.396-2.58l.051-.39c.319-2.386.328-4.18-.223-5.394-.293-.644-.743-1.125-1.355-1.431-.59-.296-1.284-.404-2.036-.404h-2.05l.056-.429c.025-.18.05-.372.076-.572.06-.483.117-1.006.117-1.438 0-1.245-.222-2.253-.92-2.941-.684-.675-1.668-.88-2.743-.956zM7 18.918c1.059.064 2.079.355 3.118.652l.568.16c1.406.39 3.006.77 5.142.77 2.277 0 3.004-.274 3.39-.781.216-.283.388-.718.54-1.448.136-.65.242-1.45.379-2.477l.05-.384c.32-2.4.253-3.795-.102-4.575-.16-.352-.375-.568-.66-.711-.305-.153-.74-.245-1.365-.245h-2.37c-.681 0-1.293-.57-1.211-1.328.026-.243.065-.537.105-.834l.07-.527c.06-.482.105-.921.105-1.25 0-1.125-.213-1.617-.473-1.873-.275-.27-.774-.455-1.795-.528-.351-.024-.698.274-.698.71v1.053c0 3.55-2.488 5.063-3.68 5.577-.372.16-.754.232-1.113.26v7.78zM3.75 20.5a.25.25 0 01-.25-.25V9.75a.25.25 0 01.25-.25h1.5a.25.25 0 01.25.25v10.5a.25.25 0 01-.25.25h-1.5z"></path></svg>
    </label>
    <input hidden="" id="helpfulness-no" type="radio" name="helpfulness-vote" value="No" aria-label="No">
    <label class="btn x-radio-label" for="helpfulness-no">
      <svg version="1.1" width="24" height="24" viewBox="0 0 24 24" class="octicon octicon-thumbsdown" aria-hidden="true"><path fill-rule="evenodd" d="M12.596 21.957c-1.301.092-2.303-.986-2.303-2.206v-1.053c0-2.666-1.813-3.785-2.774-4.2a1.864 1.864 0 00-.523-.13A1.75 1.75 0 015.25 16h-1.5A1.75 1.75 0 012 14.25V3.75C2 2.784 2.784 2 3.75 2h1.5a1.75 1.75 0 011.742 1.58c.838-.06 1.667-.296 2.69-.586l.602-.17C11.748 2.419 13.497 2 15.828 2c2.188 0 3.693.204 4.583 1.372.422.554.65 1.255.816 2.05.148.708.262 1.57.396 2.58l.051.39c.319 2.386.328 4.18-.223 5.394-.293.644-.743 1.125-1.355 1.431-.59.296-1.284.404-2.036.404h-2.05l.056.429c.025.18.05.372.076.572.06.483.117 1.006.117 1.438 0 1.245-.222 2.253-.92 2.942-.684.674-1.668.879-2.743.955zM7 5.082c1.059-.064 2.079-.355 3.118-.651.188-.054.377-.108.568-.16 1.406-.392 3.006-.771 5.142-.771 2.277 0 3.004.274 3.39.781.216.283.388.718.54 1.448.136.65.242 1.45.379 2.477l.05.385c.32 2.398.253 3.794-.102 4.574-.16.352-.375.569-.66.711-.305.153-.74.245-1.365.245h-2.37c-.681 0-1.293.57-1.211 1.328.026.244.065.537.105.834l.07.527c.06.482.105.922.105 1.25 0 1.125-.213 1.617-.473 1.873-.275.27-.774.456-1.795.528-.351.024-.698-.274-.698-.71v-1.053c0-3.55-2.488-5.063-3.68-5.577A3.485 3.485 0 007 12.861V5.08zM3.75 3.5a.25.25 0 00-.25.25v10.5c0 .138.112.25.25.25h1.5a.25.25 0 00.25-.25V3.75a.25.25 0 00-.25-.25h-1.5z"></path></svg>
    </label>
  </p>
  <p class="text-gray f6" hidden="" data-help-yes="">
    Want to learn about new docs features and updates? Sign up for updates!
  </p>
  <p class="text-gray f6" hidden="" data-help-no="">
    We're continually improving our docs. We'd love to hear how we can do better.
  </p>
  <input type="text" class="d-none" name="helpfulness-token" aria-hidden="true">
  <p hidden="" data-help-no="">
    <label class="d-block mb-1 f6" for="helpfulness-comment">
      <span>Let us know what we can do better</span>
      <span class="text-normal text-gray-light float-right ml-1">
        Optional
      </span>
    </label>
    <textarea class="form-control input-sm width-full" name="helpfulness-comment" id="helpfulness-comment"></textarea>
  </p>
  <p>
    <label class="d-block mb-1 f6" for="helpfulness-email" hidden="" data-help-no="">
      Can we contact you if we have more questions?
      <span class="text-normal text-gray-light float-right ml-1">
        Optional
      </span>
    </label>
    <input type="email" class="form-control input-sm width-full" name="helpfulness-email" id="helpfulness-email" placeholder="email@example.com" hidden="" data-help-yes="" data-help-no="">
  </p>
  <p class="text-right" hidden="" data-help-yes="" data-help-no="">
    <button type="submit" class="btn btn-blue btn-sm">
      Send
    </button>
  </p>
  <p class="text-gray f6" hidden="" data-help-end="">
    Thank you! Your feedback has been submitted.
  </p>
</form>


    </div>
    <div class="col-12 col-lg-6 col-xl-4 mb-6 mb-xl-0 float-left">
      
<div class="f5 contribution">
  <h2 class="f4">Help us make these docs great!</h2>
  <p class="text-gray f6">All GitHub docs are open source. See something that's wrong or unclear? Submit a pull request.</p>
  
    
  
  <a class="btn btn-outline" href="https://github.com/github/docs/edit/main/content/github/working-with-github-pages/creating-a-github-pages-site.md">
    <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-git-pull-request" aria-hidden="true"><path fill-rule="evenodd" d="M7.177 3.073L9.573.677A.25.25 0 0110 .854v4.792a.25.25 0 01-.427.177L7.177 3.427a.25.25 0 010-.354zM3.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122v5.256a2.251 2.251 0 11-1.5 0V5.372A2.25 2.25 0 011.5 3.25zM11 2.5h-1V4h1a1 1 0 011 1v5.628a2.251 2.251 0 101.5 0V5A2.5 2.5 0 0011 2.5zm1 10.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0zM3.75 12a.75.75 0 100 1.5.75.75 0 000-1.5z"></path></svg>
    Make a contribution
  </a>
  <p class="text-gray f6 mt-2">Or, <a href="https://github.com/github/docs/blob/main/CONTRIBUTING.md" target="_blank">learn how to contribute.</a></p>
</div>


    </div>
    <div class="col-12 col-lg-12 col-xl-4 float-left">
      <!-- Contact support banner -->
<div>
  <h3 class="mb-2 f4">
    Still need help?
  </h3>
  
  <a id="ask-community" href="https://github.community" class="btn btn-outline mr-4 mt-2">
    <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-people" aria-hidden="true"><path fill-rule="evenodd" d="M5.5 3.5a2 2 0 100 4 2 2 0 000-4zM2 5.5a3.5 3.5 0 115.898 2.549 5.507 5.507 0 013.034 4.084.75.75 0 11-1.482.235 4.001 4.001 0 00-7.9 0 .75.75 0 01-1.482-.236A5.507 5.507 0 013.102 8.05 3.49 3.49 0 012 5.5zM11 4a.75.75 0 100 1.5 1.5 1.5 0 01.666 2.844.75.75 0 00-.416.672v.352a.75.75 0 00.574.73c1.2.289 2.162 1.2 2.522 2.372a.75.75 0 101.434-.44 5.01 5.01 0 00-2.56-3.012A3 3 0 0011 4z"></path></svg>
    Ask the GitHub community
  </a>
  <a id="contact-us" href="https://support.github.com/contact" class="btn btn-outline mt-2">
    <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-comment-discussion" aria-hidden="true"><path fill-rule="evenodd" d="M1.5 2.75a.25.25 0 01.25-.25h8.5a.25.25 0 01.25.25v5.5a.25.25 0 01-.25.25h-3.5a.75.75 0 00-.53.22L3.5 11.44V9.25a.75.75 0 00-.75-.75h-1a.25.25 0 01-.25-.25v-5.5zM1.75 1A1.75 1.75 0 000 2.75v5.5C0 9.216.784 10 1.75 10H2v1.543a1.457 1.457 0 002.487 1.03L7.061 10h3.189A1.75 1.75 0 0012 8.25v-5.5A1.75 1.75 0 0010.25 1h-8.5zM14.5 4.75a.25.25 0 00-.25-.25h-.5a.75.75 0 110-1.5h.5c.966 0 1.75.784 1.75 1.75v5.5A1.75 1.75 0 0114.25 12H14v1.543a1.457 1.457 0 01-2.487 1.03L9.22 12.28a.75.75 0 111.06-1.06l2.22 2.22v-2.19a.75.75 0 01.75-.75h1a.25.25 0 00.25-.25v-5.5z"></path></svg>
    Contact support
  </a>
</div>

    </div>
  </div>
</section>

      <footer class="py-6 text-small">
  <div class="container-xl d-flex px-3 px-md-6">
    <ul class="d-flex list-style-none flex-wrap flex-justify-center flex-xl-justify-start">
      <li class="d-flex mr-xl-3 text-gray">
        <svg version="1.1" width="20" height="20" viewBox="0 0 16 16" class="octicon octicon-mark-github mr-2 mr-xl-3" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
        <span>© 2021 GitHub, Inc.</span>
      </li>
      <li class="ml-3"><a href="/github/site-policy/github-terms-of-service">Terms </a></li>
      <li class="ml-3"><a href="/github/site-policy/github-privacy-statement">Privacy </a></li>
      <li class="ml-3"><a href="https://github.com/security">Security</a></li>
      <li class="ml-3"><a href="https://www.githubstatus.com/">Status</a></li>
      <li class="ml-3"><a href="/">Help</a></li>
      <li class="ml-3"><a href="https://support.github.com">Contact GitHub</a></li>
      <li class="ml-3"><a href="https://github.com/pricing">Pricing</a></li>
      <li class="ml-3"><a href="/developers">Developer API</a></li>
      <li class="ml-3"><a href="https://services.github.com/">Training</a></li>
      <li class="ml-3"><a href="https://github.com/about">About</a></li>
    </ul>
  </div>
</footer>

<script id="expose" type="application/json">{"searchOptions":{"languages":["en","cn","ja","es","pt","de"],"versions":{"free-pro-team@latest":"dotcom","enterprise-server@3.0":"3.0","enterprise-server@2.22":"2.22","enterprise-server@2.21":"2.21","github-ae@latest":"ghae"},"nonEnterpriseDefaultVersion":"free-pro-team@latest"}}</script>
<script src="/dist/index.js?hash=38d1ea8533d1170510ced5d21e48ddd5"></script>


      <button class="arrow-for-scrolling-top show" id="js-scroll-top">
    <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-chevron-up" aria-hidden="true"><path fill-rule="evenodd" d="M3.22 9.78a.75.75 0 010-1.06l4.25-4.25a.75.75 0 011.06 0l4.25 4.25a.75.75 0 01-1.06 1.06L8 6.06 4.28 9.78a.75.75 0 01-1.06 0z"></path></svg>
</button>

    </main>
  

<div id="shimai-world" style="position: fixed; top: 0px; left: 0px; width: 100%; height: 100%; z-index: 2147483647; pointer-events: none; background: transparent;"></div></body></html>
