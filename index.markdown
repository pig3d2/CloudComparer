---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<head>
    <meta charset="utf-8">
    <link rel="icon" type="image/x-icon" href="/favicon.ico"/>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="robots" content="follow,index">
    <META NAME="Title" CONTENT="A Public Cloud Comparison | AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <META NAME="Keywords" CONTENT="AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba, AWS vs Azure, Azure vs Google">
    <META NAME="Description" CONTENT="A detailed public cloud services comparison & mapping of Amazon AWS, Microsoft Azure, Google Cloud, IBM Cloud, Oracle Cloud.">
    <META NAME="Author" CONTENT="Ilyas">
    <META NAME="Subject" CONTENT="A Public Cloud Comparison | AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <meta property="og:type" content="website">
    <meta property="og:title" content="A Public Cloud Comparison | AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <meta property="og:locale" content="en_US">
    <meta property="og:description" content="A detailed public cloud services comparison & mapping of Amazon AWS, Microsoft Azure, Google Cloud, IBM Cloud, Oracle Cloud.">
    <link rel="canonical" href="https://comparecloud.in/">
    <meta property="og:url" content="https://comparecloud.in/">
    <meta property="og:site_name" content="A Public Cloud Comparison | AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <meta property="og:image" content="/img/Logo_small.jpg">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:site" content="@Ilyas_tweets">
    <meta name="twitter:creator" content="@Ilyas_tweets">
    <meta property="article:author" content="https://www.facebook.com/IlyasTheWebizen">
    <meta name="twitter:description" content="A detailed public cloud services comparison & mapping of Amazon AWS, Microsoft Azure, Google Cloud, IBM Cloud, Oracle Cloud.">
    <meta name="twitter:title" content="A public Cloud Compareison : AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba">
    <title>AWS vs Azure vs Google vs IBM vs Oracle vs Alibaba | A detailed comparison and mapping between various cloud services</title>
</head>
<script type="text/javascript" src="https://s7.addthis.com/js/300/addthis_widget.js#pubid=ra-552c144e4f497fe9"></script>
<!-- Place this tag in your head or just before your close body tag. -->
<script async defer src="https://buttons.github.io/buttons.js"></script>
<!-- <table class="github">
<tr align="center" >
<td><!-- Place this tag where you want the button to render. -->


<table id="comparison">
  <tr align="center" class="header" style="position:sticky;top: 0">
	            <th style="width:7%">Category</th>
            <th style="width:10%">Service</th>
            <th>
              <img  src="{{ site.baseurl }}/assets/img/logo/aws.png" alt="AWS Icon" class="header-img"/>
            </th>
            <th>
              <img  src="{{ site.baseurl }}/assets/img/logo/msazure.svg" alt="Microsoft Azure Log"/>
            </th>
            <th>
              <img  src="{{ site.baseurl }}/assets/img/logo/google.svg" alt="Google Cloud Platform Logo" />
            </th>
            <th>
              <img  src="{{ site.baseurl }}/assets/img/logo/IBM-Cloud-svg-lockup-color8.svg"  alt="IBM Cloud Logo" />
            </th>
            <th>
              <img  src="{{ site.baseurl }}/assets/img/logo/oracle.png" alt="Oracle Cloud Logo"/>
            </th>
            <th>
              <img src="{{ site.baseurl }}/assets/img/logo/alibaba.png" alt="Alibaba Cloud Logo"/>
            </th>
			<th>
              <img  src="{{ site.baseurl }}/assets/img/logo/huawei.png" alt="Huawei Cloud"/>
            </th>
			<th>
              <img  src="{{ site.baseurl }}/assets/img/logo/tencentCloud.png" alt="Tencent Cloud"/>
            </th>
  </tr>
	{% for item in site.data.cloudservices.services %}
	<tr>
		<td>{{item.category}}</td>
		<td>{{item.subcategory}}</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.aws %}
						<li ><img src="{{ site.baseurl }}/assets/img/cloudproviders/aws/{{record.icon}}" alt="{{record.name}}" > <a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.azure %}
						<li><img src="{{ site.baseurl }}/assets/img/cloudproviders/azure/{{record.icon}}" alt="{{record.name}}"  ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
				{% for record in entry.google %}
					<li><img src="{{ site.baseurl }}/assets/img/cloudproviders/google/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
				{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
				{% for record in entry.ibm %}
						<li><img src="{{ site.baseurl }}/assets/img/cloudproviders/ibm/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
				{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.oracle %}
							<li ><img src="{{ site.baseurl }}/assets/img/cloudproviders/oracle/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.alibaba %}
							<li><img src="{{ site.baseurl }}/assets/img/cloudproviders/alibaba/{{record.icon}}" alt="{{record.name}}" ><a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a></li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
					{% for record in entry.huawei %}
							<li>
								<img src="{{ site.baseurl }}/assets/img/cloudproviders/huawei/{{record.icon}}" alt="{{record.name}}">
								<a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a>
							</li>
					{% endfor %}	
				{% endfor %}	
			</ul>
		</td>
		<td>
			<ul>
			    {% for entry in item.service %} 
				{% for record in entry.tencent %}
					<li>
						<img src="{{ site.baseurl }}/assets/img/cloudproviders/tencent/{{record.icon}}" alt="{{record.name}}">
						<a href="{{record.ref}}" target="_blank" alt="{{record.name}}">{{record.name}}</a>
					</li>
				{% endfor %}
			{% endfor %}
			</ul>
		</td>
	</tr>
	{% endfor %}
</table>
