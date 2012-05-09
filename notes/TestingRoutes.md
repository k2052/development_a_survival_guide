A lot of people avoid complex controller tests. And by complex I mean testing that the data spit out is correct. Typically this is done with something like Capybara. It works well but is a lot of effort if your application isn't a major site where it's absolutely critical that some text is there.

Most feel that as long as the route doesn't error then the test for a controller is adequate. I advocate a different approach than Capybara. Build json interfaces to data that you normally wouldn't provide json for. That way you can check at least that model is correct. With responders and provides this is quite easy to do. This gets you 90% of the way to a full test without needing to write html and css selectors using Capybara.

