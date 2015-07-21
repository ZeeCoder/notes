#Symfony
 - Getting the current url: (Careful, on 404 error pages it throws an Exception!)

 ```
 {{ path(
    app.request.attributes.get('_route'),
    app.request.attributes.get('_route_params') | merge({
        _locale: localeUrlPart
    })
) }}
 ```
 - Trailing slashes in routes in Sf projects explained: https://github.com/silexphp/Silex/issues/149
 - Sf3 dir structure: SENSIOLABS_ENABLE_NEW_DIRECTORY_STRUCTURE=true composer create-project symfony/framework-standard-edition myproject
 - Capifony libs: https://github.com/everzet/capifony/tree/master/lib
 - assetic versions: http://stackoverflow.com/questions/17795200/symfony2-assets-versioning-by-file
 - Sf Form Twig Blocks: https://github.com/symfony/symfony/blob/master/src/Symfony/Bridge/Twig/Resources/views/Form/form_div_layout.html.twig
 - Sf FOS User config ref https://github.com/FriendsOfSymfony/FOSUserBundle/blob/master/Resources/doc/configuration_reference.md
 - sf2 Endroid bundles: http://symfony-application.endroid.nl/
