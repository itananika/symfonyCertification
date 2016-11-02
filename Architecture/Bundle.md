## Budles
### Base information

There are two types of bundles:
1. Application-specific bundles: only used to build your application;
2. Reusable bundles: meant to be shared across many projects.


### Useful bundles list
* FrameworkBundle - The core Symfony framework bundle
* [SensioFrameworkExtraBundle](https://symfony.com/doc/current/bundles/SensioFrameworkExtraBundle/index.html) - Adds several enhancements, including template and routing annotation capability
* [TwigBundle](https://symfony.com/doc/3.0/book/templating.html) - Adds support for the Twig templating engine
* [SecurityBundle](https://symfony.com/doc/3.0/book/security.html) - Adds security by integrating Symfony's security component
* [SwiftmailerBundle](https://symfony.com/doc/2.8/email.html) - Adds support for Swiftmailer, a library for sending emails
* [MonologBundle](https://symfony.com/doc/2.6/cookbook/logging/monolog.html) - Adds support for Monolog, a logging library
* WebProfilerBundle (in dev/test env) - Adds profiling functionality and the web debug toolbar
* SensioDistributionBundle (in dev/test env) - Adds functionality for configuring and working with Symfony distributions
* [SensioGeneratorBundle](https://symfony.com/doc/3.0/bundles/SensioGeneratorBundle/index.html) (in dev/test env) - Adds code generation capabilities
* [AsseticBundle](http://symfony.com/doc/2.7/assetic/asset_management.html) -Adds support for Assetic, an asset processing library
* DebugBundle (in dev/test env) - Adds Debug and VarDumper component integration
* [BlockBundle](http://symfony.com/doc/master/cmf/bundles/block/introduction.html) - This bundle provides integration with SonataBlockBundle. It is used to manage fragments of content, so-called blocks, that are persisted in a database and can be incorporated into any page layout.
* [CoreBundle](http://symfony.com/doc/master/cmf/bundles/core/introduction.html) - This bundle provides common functionality, helpers and utilities for the other CMF bundles.
* [ContentBundle](http://symfony.com/doc/master/cmf/bundles/content/introduction.html) - The ContentBundle provides a document for static content and the controller to render any content that needs no special handling in the controller.
* [CreateBundle](http://symfony.com/doc/master/cmf/bundles/create/introduction.html) - The CreateBundle provides modern front-end in-place editing for web applications. It integrates create.js and the CreatePHP library into Symfony2.
* [MediaBundle](http://symfony.com/doc/master/cmf/bundles/media/introduction.html) - The MediaBundle provides a way to store and edit any media and provides a generic base of common interfaces and models that allow the user to build media management solutions for a CMS(very minimalistic and is focused on images and download files).
* [MenuBundle](http://symfony.com/doc/master/cmf/bundles/menu/introduction.html) - The CmfMenuBundle extends the KnpMenuBundle and adds the following features: Render menus stored in the persistence layer; Generate menu node URLs from linked Content or Route. Note that only the Doctrine PHPCR-ODM persistence layer is currently supported.
* [RoutingBundle](http://symfony.com/doc/master/cmf/bundles/routing/introduction.html) - The RoutingBundle integrates dynamic routing into Symfony using the CMF Routing component . See the component documentation if you are interested in the implementation details of the services explained in this chapter.
* [SearchBundle](http://symfony.com/doc/master/cmf/bundles/search/introduction.html) - The SearchBundle provides integration with LiipSearchBundle to provide a site wide search.
* [SeoBundle](http://symfony.com/doc/master/cmf/bundles/seo/introduction.html) - This bundle provides a layer on top of the SonataSeoBundle, to make it easier to collect SEO data from content documents.
* [SimpleCmsBundle](http://symfony.com/doc/master/cmf/bundles/simple_cms/introduction.html) - The SimpleCmsBundle provides a simplistic CMS on top of the CMF components and bundles.
* [TreeBrowserBundle](http://symfony.com/doc/master/cmf/bundles/tree_browser/introduction.html) - The TreeBrowserBundle provides a tree navigation on top of a PHPCR repository. The front-end implementation is based on the jQuery plugin jsTree.
* [SonataDoctrinePHPCRAdminBundle]() - The Doctrine PHPCR-ODM Admin integrates the Admin Bundle with the [Doctrine PHPCR-ODM](http://symfony.com/doc/master/cmf/bundles/phpcr_odm/introduction.html) project.
* [FOSUserBundle (60%)](https://github.com/FriendsOfSymfony/FOSUserBundle) - The FOSUserBundle adds support for a database-backed user system in Symfony2. It provides a flexible framework for user management that aims to handle common tasks such as user registration and password retrieval.
* [FOSRestBundle (30%)](https://github.com/FriendsOfSymfony/FOSRestBundle) - This bundle provides various tools to rapidly develop RESTful API's & applications with Symfony.
* [KnpMenuBundle (25%)](https://github.com/KnpLabs/KnpMenuBundle) - The KnpMenuBundle integrates the KnpMenu PHP library with Symfony. This means easy-to-implement and feature-rich menus in your Symfony application!
* [StofDoctrineExtensionsBundle (25%)](https://github.com/stof/StofDoctrineExtensionsBundle) - This bundle provides integration for DoctrineExtensions in your Symfony2 Project.
* [DoctrineBundle](https://symfony.com/doc/current/bundles/DoctrineBundle/index.html) - Integrates Doctrine's ORM and DBAL projects into Symfony applications. It provides configuration options, console commands and even a web debug toolbar collector.
* [DoctrineFixturesBundle](https://symfony.com/doc/current/bundles/DoctrineFixturesBundle/index.html) - Fixtures are used to load a controlled set of data into a database. This data can be used for testing or could be the initial data required for the application to run smoothly. Symfony has no built in way to manage fixtures but Doctrine2 has a library to help you write fixtures for the Doctrine ORM or ODM.
* [DoctrineMongoDBBundle](https://symfony.com/doc/current/bundles/DoctrineMongoDBBundle/index.html) - The MongoDB Object Document Mapper (ODM) is much like the Doctrine2 ORM in its philosophy and how it works. In other words, like the Doctrine2 ORM, with the Doctrine ODM, you deal only with plain PHP objects, which are then persisted transparently to and from MongoDB.
* [DoctrineMigrationsBundle](https://symfony.com/doc/current/bundles/DoctrineMigrationsBundle/index.html) - The database migrations feature is an extension of the database abstraction layer and offers you the ability to programmatically deploy new versions of your database schema in a safe, easy and standardized way.
* [DoctrineCacheBundle](https://symfony.com/doc/current/bundles/DoctrineCacheBundle/index.html) - The Doctrine Common caching library was born from a need in the Doctrine2 ORM to allow caching of result sets. The library is independent and can be used in your own libraries and applications to implement caching.
* [JMSSerializerBundle (24%)](https://github.com/schmittjoh/JMSSerializerBundle) - This bundle integrates the serializer library into Symfony2.
* [SonataAdminBundle (24%)](https://github.com/sonata-project/SonataAdminBundle) - The missing Symfony Admin Generator
* [FOSJsRoutingBundle (23%)](https://github.com/FriendsOfSymfony/FOSJsRoutingBundle) - This bundle allows you to expose your routing in your JavaScript code. That means you'll be able to generate URL with given parameters like you can do with the Router component provided in the Symfony2 core.
* [LiipImagineBundle (22%)](https://github.com/liip/LiipImagineBundle) - This bundle provides an image manipulation abstraction toolkit for Symfony-based projects.
* [IvoryCKEditorBundle](https://symfony.com/doc/current/bundles/IvoryCKEditorBundle/index.html) - The bundle integrates CKEditor into Symfony via the Form Component. It automatically registers a new type called ckeditor which can be fully configured. This type extends the textarea one, meaning all textarea options are available.
* [KnpPaginatorBundle (16%)](https://github.com/KnpLabs/KnpPaginatorBundle) - SEO friendly Symfony2 paginator to paginate everything. Generally this bundle is based on Knp Pager component. This component introduces a different way for pagination handling. You can read more about the internal logic on the given documentation link.
* [NelmioApiDocBundle (11%)](https://github.com/nelmio/NelmioApiDocBundle) - The NelmioApiDocBundle bundle allows you to generate a decent documentation for your APIs.
* [FOSElasticaBundle (11%)](https://github.com/FriendsOfSymfony/FOSElasticaBundle) - This bundle provides integration with ElasticSearch and Elastica with Symfony2.
* [KnpSnappyBundle (8%)](https://github.com/KnpLabs/KnpSnappyBundle) - Snappy is a PHP (5.3+) wrapper for the wkhtmltopdf conversion utility. It allows you to generate either pdf or image files from your html documents, using the webkit engine. The KnpSnappyBundle provides a simple integration for your Symfony project.
* [JMSTranslationBundle (3%)](https://github.com/schmittjoh/JMSTranslationBundle) - This bundle puts the Symfony Translation Component on steroids. While the Translation component is highly optimized to reduce the runtime overhead of your code, it lacks a few features for translators. The aim of this bundle is to make translating a site easier while still retaining all of the performance optimizations that are currently in place.


[Useful Link 1](https://github.com/sitepoint/awesome-symfony)