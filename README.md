# Magento2CustomBlockINCMS
Magento2 add any core or custom block in CMS from admin panel

#Steps for adding  block into CMS for example add CatalogSearch/Advance search on 404 page

1. Login into admin panel using existing credentials
2. Open Content->pages and edit 404 page
3. Design-> Layout Update XML
4. Add XML content for Advacne search
 
 <referenceContainer name="content">
    <block class="Magento\CatalogSearch\Block\Advanced\Form" name="catalogsearch_advanced_form" template="Magento_CatalogSearch::advanced/form.phtml"/>
    <block class="Magento\Framework\View\Element\Html\Calendar" name="html_calendar" as="html_calendar" template="Magento_Theme::js/calendar.phtml"/>
 </referenceContainer>