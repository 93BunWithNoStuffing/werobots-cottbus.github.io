---
title: Search
search: exclude
permalink: search
folder: search
hide_sidebar: true
toc: false
---

<!--start search-->
<input type="text" id="_search-input" placeholder="suchen ...">
<ol id="onpage_results-container"></ol>

<script src="{{ '_scripts/jekyll-search.js' }}" type="text/javascript"></script>
<script type="text/javascript">
	SimpleJekyllSearch.init({
		searchInput: document.getElementById('_search-input'),
		resultsContainer: document.getElementById('onpage_results-container'),
		dataSource: '{{ "search.json" }}',
		searchResultTemplate: '<li><a href="{url}" style="font-size: 110%;">{title}</a><br><span style="font-size: 80%;">{date}&nbsp;&minus;&nbsp;{path}</span></li>',
		noResultsText: '{{ site.data.strings.search_no_results_text }}',
		fuzzy: true
	})
</script>
<!--end search-->
