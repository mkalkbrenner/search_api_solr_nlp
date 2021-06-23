# Search API Solr NLP

Search API Solr NLP adds support for Solr's OpenNLP integration to Search API
Solr.

Due to the requirement for trained models for natural language processing that
might take a lot of space, this functionality encapsulated in an optional module
and not included in Search API Solr itself.

Search API Solr NLP adds some new fulltext field types to Solr config sets, for
example "nouns". Using this field type you can filter any text for nouns. The
resulting data stored in the index is great source for features like
auto complete or spell check.

## Installation

This module has to be installed via composer to pull its dependencies. These
contain a set of pre-trained models for different languages from apache.org. The
first download ever of these files takes some time. Composer isn't fast on
fetching those files. So it isn't an error when the first time download takes
longer! Afterwards these files are cached.
