# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `Appo - Angular 9 App Landing Page` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'appo';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { HeroOneComponent } from './components/hero/hero-one/hero-one.component';
import { HeroTwoComponent } from './components/hero/hero-two/hero-two.component';
import { HeroThreeComponent } from './components/hero/hero-three/hero-three.component';
import { HeroFourComponent } from './components/hero/hero-four/hero-four.component';
import { HeroFiveComponent } from './components/hero/hero-five/hero-five.component';
import { HeroSixComponent } from './components/hero/hero-six/hero-six.component';
import { HeroSevenComponent } from './components/hero/hero-nine/hero-seven/hero-seven.component';
import { HeroEightComponent } from './components/hero/hero-eight/hero-eight.component';
import { HeroNineComponent } from './components/hero/hero-nine/hero-nine.component';
import { PromoOneComponent } from './components/promo/promo-one/promo-one.component';
import { PromoTwoComponent } from './components/promo/promo-two/promo-two.component';
import { AboutComponent } from './components/about/about.component';
import { WorkComponent } from './components/work/work.component';
import { FeaturesComponent } from './components/features/features.component';
import { ScreenshotComponent } from './components/screenshot/screenshot.component';
import { PricingComponent } from './components/pricing/pricing.component';
import { ReviewsComponent } from './components/reviews/reviews.component';
import { TeamComponent } from './components/team/team.component';
import { NewsletterComponent } from './components/newsletter/newsletter.component';
import { DownloadComponent } from './components/download/download.component';
import { BlogComponent } from './components/blogs/blog/blog.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { ContactComponent } from './components/contact/contact.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { PreloaderComponent } from './components/preloader/preloader.component';
import { FooterComponent } from './components/footer/footer.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { ThemeSevenComponent } from './themes/theme-seven/theme-seven.component';
import { ThemeEightComponent } from './themes/theme-eight/theme-eight.component';
import { ThemeNineComponent } from './themes/theme-nine/theme-nine.component';
import { BrandingComponent } from './components/branding/branding.component';
import { HeaderOneComponent } from './components/header/header-one/header-one.component';
import { HeaderTwoComponent } from './components/header/header-two/header-two.component';
import { LoginComponent } from './components/accounts/login/login.component';
import { SignupComponent } from './components/accounts/signup/signup.component';
import { ResetComponent } from './components/accounts/reset/reset.component';
import { AboutPageComponent } from './components/inner-pages/about-page/about-page.component';
import { SkillsComponent } from './components/skills/skills.component';
import { PromoThreeComponent } from './components/promo/promo-three/promo-three.component';
import { PricingPageComponent } from './components/inner-pages/pricing-page/pricing-page.component';
import { ReviewsPageComponent } from './components/inner-pages/reviews-page/reviews-page.component';
import { DownloadPageComponent } from './components/inner-pages/download-page/download-page.component';
import { ThankYouComponent } from './components/inner-pages/thank-you/thank-you.component';
import { NewsletterPageComponent } from './components/inner-pages/newsletter-page/newsletter-page.component';
import { ErrorOneComponent } from './components/inner-pages/error-page/error-one/error-one.component';
import { ErrorTwoComponent } from './components/inner-pages/error-page/error-two/error-two.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { MaintenanceComponent } from './components/inner-pages/maintenance/maintenance.component';
import { ComingSoonComponent } from './components/inner-pages/coming-soon/coming-soon.component';
import { BreadcrumbAboutComponent } from './components/breadcrumb/breadcrumb-about/breadcrumb-about.component';
import { BreadcrumbPricingComponent } from './components/breadcrumb/breadcrumb-pricing/breadcrumb-pricing.component';
import { BreadcrumbReviewsComponent } from './components/breadcrumb/breadcrumb-reviews/breadcrumb-reviews.component';
import { BreadcrumbFaqComponent } from './components/breadcrumb/breadcrumb-faq/breadcrumb-faq.component';
import { BreadcrumbContactComponent } from './components/breadcrumb/breadcrumb-contact/breadcrumb-contact.component';
import { BreadcrumbBlogTwoColumnComponent } from './components/breadcrumb/breadcrumb-blog-two-column/breadcrumb-blog-two-column.component';
import { BreadcrumbBlogThreeColumnComponent } from './components/breadcrumb/breadcrumb-blog-three-column/breadcrumb-blog-three-column.component';
import { BreadcrumbBlogLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-left-sidebar/breadcrumb-blog-left-sidebar.component';
import { BreadcrumbBlogRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-right-sidebar/breadcrumb-blog-right-sidebar.component';
import { BreadcrumbBlogDetailsLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-left-sidebar/breadcrumb-blog-details-left-sidebar.component';
import { BreadcrumbBlogDetailsRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-right-sidebar/breadcrumb-blog-details-right-sidebar.component';
import { FaqComponent } from './components/faq/faq.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { MapComponent } from './components/map/map.component';
import { AboutUsComponent } from './components/about-us/about-us.component';

@NgModule({
  declarations: [
    AppComponent,
    HeroOneComponent,
    HeroTwoComponent,
    HeroThreeComponent,
    HeroFourComponent,
    HeroFiveComponent,
    HeroSixComponent,
    HeroSevenComponent,
    HeroEightComponent,
    HeroNineComponent,
    PromoOneComponent,
    PromoTwoComponent,
    AboutComponent,
    WorkComponent,
    FeaturesComponent,
    ScreenshotComponent,
    PricingComponent,
    ReviewsComponent,
    TeamComponent,
    NewsletterComponent,
    DownloadComponent,
    BlogComponent,
    BlogTwoColumnComponent,
    BlogThreeColumnComponent,
    BlogLeftSidebarComponent,
    BlogRightSidebarComponent,
    BlogDetailsLeftSidebarComponent,
    BlogDetailsRightSidebarComponent,
    ContactComponent,
    ThemeOneComponent,
    ScrollupComponent,
    PreloaderComponent,
    FooterComponent,
    ThemeTwoComponent,
    ThemeThreeComponent,
    ThemeFourComponent,
    ThemeFiveComponent,
    ThemeSixComponent,
    ThemeSevenComponent,
    ThemeEightComponent,
    ThemeNineComponent,
    BrandingComponent,
    HeaderOneComponent,
    HeaderTwoComponent,
    LoginComponent,
    SignupComponent,
    ResetComponent,
    AboutPageComponent,
    SkillsComponent,
    PromoThreeComponent,
    PricingPageComponent,
    ReviewsPageComponent,
    DownloadPageComponent,
    ThankYouComponent,
    NewsletterPageComponent,
    ErrorOneComponent,
    ErrorTwoComponent,
    ContactPageComponent,
    MaintenanceComponent,
    ComingSoonComponent,
    BreadcrumbAboutComponent,
    BreadcrumbPricingComponent,
    BreadcrumbReviewsComponent,
    BreadcrumbFaqComponent,
    BreadcrumbContactComponent,
    BreadcrumbBlogTwoColumnComponent,
    BreadcrumbBlogThreeColumnComponent,
    BreadcrumbBlogLeftSidebarComponent,
    BreadcrumbBlogRightSidebarComponent,
    BreadcrumbBlogDetailsLeftSidebarComponent,
    BreadcrumbBlogDetailsRightSidebarComponent,
    FaqComponent,
    FaqPageComponent,
    MapComponent,
    AboutUsComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
    |-- theme-two ( demo theme 2)
    .....
    |-- theme-nine ( demo theme 9 )
```

`themes` folder contains all of our 9 demos.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { Routes, RouterModule } from '@angular/router';

import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { ThemeSevenComponent } from './themes/theme-seven/theme-seven.component';
import { ThemeEightComponent } from './themes/theme-eight/theme-eight.component';
import { ThemeNineComponent } from './themes/theme-nine/theme-nine.component';
import { LoginComponent } from './components/accounts/login/login.component';
import { SignupComponent } from './components/accounts/signup/signup.component';
import { ResetComponent } from './components/accounts/reset/reset.component';
import { AboutPageComponent } from './components/inner-pages/about-page/about-page.component';
import { PricingPageComponent } from './components/inner-pages/pricing-page/pricing-page.component';
import { ReviewsPageComponent } from './components/inner-pages/reviews-page/reviews-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { DownloadPageComponent } from './components/inner-pages/download-page/download-page.component';
import { ThankYouComponent } from './components/inner-pages/thank-you/thank-you.component';
import { NewsletterPageComponent } from './components/inner-pages/newsletter-page/newsletter-page.component';
import { ErrorOneComponent } from './components/inner-pages/error-page/error-one/error-one.component';
import { ErrorTwoComponent } from './components/inner-pages/error-page/error-two/error-two.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { MaintenanceComponent } from './components/inner-pages/maintenance/maintenance.component';
import { ComingSoonComponent } from './components/inner-pages/coming-soon/coming-soon.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';


const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'theme-two', component: ThemeTwoComponent},
  {path: 'theme-three', component: ThemeThreeComponent},
  {path: 'theme-four', component: ThemeFourComponent},
  {path: 'theme-five', component: ThemeFiveComponent},
  {path: 'theme-six', component: ThemeSixComponent},
  {path: 'theme-seven', component: ThemeSevenComponent},
  {path: 'theme-eight', component: ThemeEightComponent},
  {path: 'theme-nine', component: ThemeNineComponent},
  {path: 'login', component: LoginComponent},
  {path: 'signup', component: SignupComponent},
  {path: 'reset', component: ResetComponent},
  {path: 'about-page', component: AboutPageComponent},
  {path: 'pricing-page', component: PricingPageComponent},
  {path: 'reviews-page', component: ReviewsPageComponent},
  {path: 'faq-page', component: FaqPageComponent},
  {path: 'download-page', component: DownloadPageComponent},
  {path: 'thank-you', component: ThankYouComponent},
  {path: 'newsletter-page', component: NewsletterPageComponent},
  {path: 'error-one', component: ErrorOneComponent},
  {path: 'error-two', component: ErrorTwoComponent},
  {path: 'contact-page', component: ContactPageComponent},
  {path: 'maintenance', component: MaintenanceComponent},
  {path: 'coming-soon', component: ComingSoonComponent},
  {path: 'blog-two-column', component: BlogTwoColumnComponent},
  {path: 'blog-three-column', component: BlogThreeColumnComponent},
  {path: 'blog-left-sidebar', component: BlogLeftSidebarComponent},
  {path: 'blog-right-sidebar', component: BlogRightSidebarComponent},
  {path: 'blog-details-left-sidebar', component: BlogDetailsLeftSidebarComponent},
  {path: 'blog-details-right-sidebar', component: BlogDetailsRightSidebarComponent}
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `hero` , `footer` folder where we wrote our different styled component. For example `hero` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- hero ( welcome component folder )
        - hero-one ( main demo hero section )
        - hero-two ( demo two hero section )
        ...... ( and other )
    ...    
```

### Contact Page component
`inner-pages/contact-page/contact-page.component.html`

```text
|-- components
    ....
    ..
    |-- inner-pages ( all inner-pages folder )
        ......
        - contact-page ( contact-page component )
        ...... ( and other )
    ...    
```

```html
<div class="contact-page">
    <app-scrollup></app-scrollup>
    <div class="all-area">
        <app-header-one></app-header-one>
        <app-breadcrumb-contact></app-breadcrumb-contact>
        <app-contact></app-contact>
        <app-map></app-map>
        <app-footer></app-footer>
    </div>
</div>
```


## theme installtion
To install the theme you have to install [angular](https://cli.angular.io/) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build --prod
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)
