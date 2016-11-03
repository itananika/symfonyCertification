## 1. Symfony Standard Edition
Fully-functional Symfony application that you can use as the skeleton for your new applications.
#### Bundless
* FrameworkBundle - The core Symfony framework bundle
* [SensioFrameworkExtraBundle](https://symfony.com/doc/current/bundles/SensioFrameworkExtraBundle/index.html) - Adds several enhancements, including template and routing annotation capability
* [DoctrineBundle](https://symfony.com/doc/3.0/book/doctrine.html) - Adds support for the Doctrine ORM
* [TwigBundle](https://symfony.com/doc/3.0/book/templating.html) - Adds support for the Twig templating engine
* [SecurityBundle](https://symfony.com/doc/3.0/book/security.html) - Adds security by integrating Symfony's security component
* [SwiftmailerBundle](https://symfony.com/doc/2.8/email.html) - Adds support for Swiftmailer, a library for sending emails
* [MonologBundle](https://symfony.com/doc/2.6/cookbook/logging/monolog.html) - Adds support for Monolog, a logging library
* WebProfilerBundle (in dev/test env) - Adds profiling functionality and the web debug toolbar
* SensioDistributionBundle (in dev/test env) - Adds functionality for configuring and working with Symfony distributions
* [SensioGeneratorBundle](https://symfony.com/doc/3.0/bundles/SensioGeneratorBundle/index.html) (in dev/test env) - Adds code generation capabilities
* DebugBundle (in dev/test env) - Adds Debug and VarDumper component integration

## 2. Symfony Demo Application
The "Symfony Demo Application" is a reference application created to show how to develop Symfony applications following the recommended best practices.
#### Bundless
* [Symfony standart Edition bundless](https://github.com/symfony/symfony-standard)
* AcmeDemoBundle (in dev/test env) - A demo bundle with some example code

## 3. Symfony CMF Standard Edition
The Symfony CMF Standard Edition (SE) is a distribution of the Symfony Content Management Framework (CMF) and licensed under the MIT License.
This distribution is based on all the main CMF components needed for most common use cases, and can be used to create a new Symfony/CMF project from scratch.
#### Bundless
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


## 4. Symfony REST Edition
Welcome to the Symfony REST Edition - a fully-functional Symfony2 application that you can use as the skeleton for your new applications.
#### Bundless
* FrameworkBundle - The core Symfony framework bundle
* [SensioFrameworkExtraBundle](https://symfony.com/doc/current/bundles/SensioFrameworkExtraBundle/index.html) - Adds several enhancements, including template and routing annotation capability
* [DoctrineBundle](https://symfony.com/doc/3.0/book/doctrine.html) - Adds support for the Doctrine ORM
* [TwigBundle](https://symfony.com/doc/3.0/book/templating.html) - Adds support for the Twig templating engine
* [SwiftmailerBundle](https://symfony.com/doc/2.8/email.html) - Adds support for Swiftmailer, a library for sending emails
* [SecurityBundle](https://symfony.com/doc/3.0/book/security.html) - Adds security by integrating Symfony's security component
* [MonologBundle](https://symfony.com/doc/2.6/cookbook/logging/monolog.html) - Adds support for Monolog, a logging library
* [AsseticBundle](http://symfony.com/doc/2.7/assetic/asset_management.html) -Adds support for Assetic, an asset processing library
* WebProfilerBundle (in dev/test env) - Adds profiling functionality and the web debug toolbar
* SensioDistributionBundle (in dev/test env) - Adds functionality for configuring and working with Symfony distributions
* [SensioGeneratorBundle](https://symfony.com/doc/3.0/bundles/SensioGeneratorBundle/index.html) (in dev/test env) - Adds code generation capabilities
* AcmeDemoBundle (in dev/test env) - A demo bundle with some example code
* [FOSRestBundle](https://github.com/FriendsOfSymfony/FOSRestBundle) - Adds rest functionality
* [FOSHttpCacheBundle](https://github.com/FriendsOfSymfony/FOSHttpCacheBundle/) - This bundle offers tools to improve HTTP caching with Symfony2
* [NelmioApiDocBundle](https://github.com/nelmio/NelmioApiDocBundle) - Add API documentation features
* [BazingaHateoasBundle](https://github.com/willdurand/BazingaHateoasBundle) - Adds HATEOAS support. Hateoas leverages the Serializer library to provide a nice way to build HATEOAS REST web services. HATEOAS stands for Hypermedia as the Engine of Application State, and adds hypermedia links to your representations
* [HautelookTemplatedUriBundle](https://github.com/hautelook/TemplatedUriBundle) - Adds Templated URIs (RFC 6570) support
* [BazingaRestExtraBundle](https://github.com/willdurand/BazingaRestExtraBundle) - This bundle provides extra features for your REST APIs built using Symfony2.
* [JMSSerializerBundle](https://github.com/schmittjoh/serializer)