# grails-datepickerUI
Version 0.1 - 27/02/2014

A datepicker based on JQuery datepicker (http://jqueryui.com/datepicker/) and (mostly) compatible with the Grails framework

Parameters:
- name		: will be used as name and if for the actual input field
- value		: default value
- option	: options to pass to datepicker {key1: value1, key2: value2, ...}. See API: http://api.jqueryui.com/datepicker/
- locale	: locale to be used. If not passed, it will take the grails session's locale (first two letters). jquery.datepicker's locale files should be available to your app: https://github.com/jquery/jquery-ui/tree/master/ui/i18n
- class		: HTML classes to apply to the visible field
- required	: HTML required attribute

Setup:
- make sure JQuery-UI and JQuery are installed
- put this class in your grails-app/tablib folder

Example: 
	<g:datepickerUI name="myDate" required="true" value="${myDomainClass?.myDate?:new Date()}" options="{minDate:'0', maxDate:'+10Y'}" class="form-control"/>

Tested with:
- JQuery-1.11.1
- JQueryUI-1.11.3 
- Grails 2.4.4
