# Product-Revies-


# Add reviews to your product pages
# This code snippet displays reviews on your product pages and adds SEO-friendly review scores to your Google search results.

# Copy the following code snippet to your clipboard:


<div id="shopify-product-reviews" data-id="{{product.id}}">{{ product.metafields.spr.reviews }}</div>



# Paste the snippet in your sections/product-template.liquid file where you want your reviews to appear. Usually this is just below the product.description tag, the code may look something like this:

<div class="product-single__description rte" itemprop="description">
  {{ product.description }}
</div>

<div id="shopify-product-reviews" data-id="{{product.id}}">{{ product.metafields.spr.reviews }}</div>

{% if section.settings.show_share_buttons %}
  {% include 'social-sharing', share_title: product.title, share_permalink: product.url, share_image: product %}
{% endif %}

# Once added, save your theme.



#  Show Product Review's on products page, copy my code & paste where you want to show review star ratings:- 
<span class="shopify-product-reviews-badge" data-id="{{ product.id }}"></span>


Star Ratings:- <span class="shopify-product-reviews-badge" data-id="{{ product.id }}"></span>


