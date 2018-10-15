$(document).ready(function() {
    $('.function_ref').wrap(function() {
        return '<a href="/Reference/' + ($(this).attr('link') ?  $(this).attr('link') : $(this).text()) + '/"></a>';
    });

    var CCcredits =
        '<p><br/><a href="/Reference">Reference Home</a></p>' +
        '<p><em>Corrections, suggestions, and new documentation should be posted to the <a href="http://forum.z-wave.me/viewforum.php?f=3427">Forum</a>.</em></p>' +
        '<p>The text of the Z-Uno reference is based on <a href="http://www.arduino.cc/en/Reference/HomePage" target="_blank">Arduino Reference</a> and is licensed under a <a href="http://creativecommons.org/licenses/by-sa/3.0/" target="_blank">Creative Commons Attribution-ShareAlike 3.0 License</a>. Code samples in the reference are released into the public domain.</p>';
        
    var CCcreditsProj = 
        '<p><br/>Examples and projects on this site are licensed under a <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank">Creative Commons Attribution 4.0 License</a>.</p>';
        
    var loc = '/Reference';
    if (document.location.pathname.substr(0, loc.length).toLowerCase() === loc.toLowerCase()) {
        $('#page').append(CCcredits);
    }

    var loc = '/Examples';
    if (document.location.pathname.substr(0, loc.length).toLowerCase() === loc.toLowerCase()) {
        $('#page').append(CCcreditsProj);
    }
    
    $('h1[link],h2[link],h3[link],h4[link],h5[link]').each(function() {
        $(this).append(' <a name="' + $(this).attr('link') + '"></a><a href="#' + $(this).attr('link') + '"><font style="font-size: 50%; vertical-align: middle;">&#128279;</font></a>');
    });
});
