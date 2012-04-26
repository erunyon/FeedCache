PHP FeedCache
=============

How to use
-----------

Include FeedCache.php in your script

Then simply pass in the local file-name (that you want to save it as) and the remote feed:

```php
  $feed_cache = new FeedCache('local_file.xml', 'http://example.com/feed.xml');
  $data = simplexml_load_string($feed_cache->get_data());
```
You will also need to make sure you have a writable folder called "cache" in the root of your site.

Changelog
---------

* v1 (2012-04-26)
** ADD: Initial commit

License
-------

FeedCache is released under the MIT license. I make no guarantees about the reliability of this script. Use at your own risk.
