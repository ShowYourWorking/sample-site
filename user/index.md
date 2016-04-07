---
layout: page
root: ..
title: Use
---

These pages contain information on how to 
use {{ site.software_name }} i.e. contain our current adapted end-user documentation.

((TODO altered functionality and screenshots to be accounted for))

##Using ShowYourWorking

((TODO convert the current HTML to markdown to allow easy editing and sub-title anchoring))

((TODO separate out generic-use user steps from chemireg-sprecific usage steps))

<div class="row mt">
    <div class="col-sm-8 col-sm-offset-2"  style="padding-left:15px;">
        
        <h2 class="blue">ChemBio Hub platform Help section<br><small>How-tos, information and FAQs</small></h2> 
            
    </div>

</div>



<div class="row">
    <div class="col-sm-8 col-sm-offset-2" data-spy="scroll" style="position: relative;">

        <div class="row">
            <div class="col-xs-12">
                <div class="well text-center">
                    <em>Jump to</em>: <a ng-click="scrollTo('overview')"><strong class="nexa">Data Overview</strong></a> | <a ng-click="scrollTo('adding-data')"><strong class="nexa">Adding data</strong></a> | <a ng-click="scrollTo('searching')"><strong class="nexa">Searching AssayReg</strong></a> | <a ng-click="scrollTo('chembl')"><strong class="nexa">Depositing data to Chembl </strong></a> | <a ng-click="scrollTo('chemireg-section')"><strong class="nexa">Adding Chemical Data</strong></a> 
                </div>
                
                
                <h2 class="blue" id="problem">What to do if you have a problem</h2>
                <p><strong class="nexa blue">If you encounter a problem with AssayReg, and this help document does not provide the answer please use the AssayReg menu box to submit an issue - click the AssayReg logo and select <em>Report an Issue</em> Alternatively please email ChemBio Hub - <a href="mailto:info@chembiohub.ox.ac.uk" role="button" class="btn btn-default"><span class="glyphicon glyphicon-envelope"></span> info@chembiohub.ox.ac.uk</a></strong></p>

                <h2 class="blue" id="loggingin">Logging in and initial screen</h2>
                <p>When you log onto AssayReg, you will see a list of the projects you have been given access to. If you think you should be able to access a project not shown in this list, please contact ChemBio Hub <a href="mailto:info@chembiohub.ox.ac.uk" role="button" class="btn btn-default"><span class="glyphicon glyphicon-envelope"></span> info@chembiohub.ox.ac.uk</a> </p>
                <p>Each project has a number of options available:
                    <img src="{{ site.baseurl }}/assets/images/help/project-list-item.png" class="img img-responsive center-block">
                    <ul>
                        <!-- <li><strong>Project Data Overview</strong> - click the project title to be taken to the Project Data Overview page;</li> -->
                        <li><strong>Assay</strong> - click <strong>Data Overview</strong> to be taken to the Project Data Overview page;</li>
                        <li><strong>Chem</strong> - you can <strong>Add Compounds</strong> if you have the correct permissions or <strong>Search Compounds</strong></li>
                    </ul>
                </p>

                <h2 class="blue" id="overview">Project Data Overview</h2>
                <p>For each project, there is a data overview page. This displays all of the data present in the project, separated out into three levels: <strong>Sub-Project</strong>, <strong>Assay</strong> and <strong>Activity</strong>.</p>

                <h3 class="blue" id="sections-explained">Project sections - an explanation</h3>
                <p>Each Project contains 3 sections:
                    <ul>
                        <li><strong>Sub-Project</strong> - A sub-project normally holds details for a collection of different assays, for example a set of different Characterisation experiments on a particular drug target.</li>
                        <li><strong>Assay</strong> - An assay normally holds details of experimental protocols and method development, for example data which needs to be provided to make the assay reproducible. Assays can belong to multiple different Sub-Projects.</li>
                        <li><strong>Activity</strong> - An activity holds the single outcome of an Assay, usually machine readouts or more qualitative data. Activity data is specific to a given Assay.</li>
                    </ul>
                </p>

                <h3 class="blue" id="show-details">Show details</h3>
                <p>You can see the data for a particular level by clicking the appropriate <strong>Actions</strong> button and clicking View Details. This will open a popup window.</p>
                <p><img src="assets/images/help/view-details.png" class="img img-responsive center-block"> <img src="{{ site.baseurl }}/assets/images/help/details-modal.png" class="img img-responsive center-block"></p>
                <p></p>

                <h3 class="blue">Editing</h3>
                <p>If you have the correct privileges, you can edit data at the Project, Sub Project or Assay level. Click the appropriate <strong>Actions</strong> button and click Edit. A popup window will launch with editable fields containing the data. Make your changes and click <strong>Update and Close</strong>.</p>

                <h3 class="blue">Duplicating</h3>
                <p>If you have the correct privileges, you can duplicate data at the Project, Sub Project or Assay level. Click the appropriate <strong>Actions</strong> button and click Duplicate. A form will be displayed, similar to the Add Single form (discussed below), with editable fields containing the data. Make any changes, add new data if needed and click <strong>Submit</strong>. this will create a new entity which will be displayed in the Data Overview page.</p>

                <h3 class="blue" >Activity</h3>
                <p>Activity data for a particular assay is displayed as a table. You can page through the data easily using the buttons at the bottom of the table. If your table contains a lot of columns, you can use the horizontal scrollbar.</p>
                <p>Each row of the Activities table contains a <strong>Duplicate</strong> link in the first column. This allows you to add a new Activity record via the Add Single Activity form, with the data from this row prepopulated into the form. Adding Data is discussed in more depth below.</p>
                <p>If your Activity data references a specific compound, an image of that structure will be shown, provided the UOX ID is registered in this project.</p>

                <h3 class="blue" >Filtering activities</h3>
                <p><img src="{{ site.baseurl }}/assets/images/help/filter-and-download.png" class="img img-responsive center-block"></p>
                <p></p> 
                <p>At the top of the Activities section is a filter text box. So for example, if you type "dichloro" into the text box, the Activities table will only show rows that contain "dichloro" in any of the columns.</p>

                <h3 class="blue" >Export</h3>
                <p>The <strong>Download</strong> button allows you to download all the results in the table as an Excel file. To download all activity records, ensure the filter text box is blank. Any filteringapplied will be reflected in the exported file.</p>

                <h2 class="blue" id="adding-data">Adding data</h2>
                <p>If you have the correct permissions, you can add data to the system through the AssayReg user interface.</p>

                <h3 class="blue" >Single record</h3>
                <p>Adding a single record is the simplest means of getting data into the system. Click <strong>Add Single Activity</strong> and select the correct Assay template to use from the list shown.</p>
                <p><img src="{{ site.baseurl }}/assets/images/help/single-activity-button.png" class="img img-responsive center-block"></p>
                <p>A form is then displayed with a placeholder for each field defined in this specific assay. Some fields will be limited in what can be input- for example dates will show a datepicker/calendar field.</p>
                <p><img src="{{ site.baseurl }}/assets/images/help/single-activity.png" class="img img-responsive center-block"></p>
                <p>When you have added the necessary data, click the Submit button. Your data will be saved and will be vsible in the Activity table.</p>

                <h3 class="blue" >Multiple records (via upload)</h3>
                <p>You can add multiple records to AssayReg from an Excel file. To use an accurate list of all relevant fields for the specific assay you can download a template of the data format by clicking <strong>Upload Multiple Activities</strong> then click <strong>Download (activity) Template</strong>. You can then use this to add your data for a smooth upload.</p>

                <p>If you have data in a different spreadsheet format, for example from another lab or from machine outputs, you can also upload that data but you may need to map some or all your data, which is explained later in this document. </p>

                <p>For simple file uploads, follow these steps:<br>
                    <ul>
                        <li>
                            Within the Sub-project and Assay you wish to register the data to, select ‘Upload Multiple Activities’. Select the Assay definition relevant to your data.<br>
                            <p><img src="{{ site.baseurl }}/assets/images/help/multiple-activities-1.png" class="img img-responsive center-block"><br></p>
                        </li>   
                        <li>
                            Drag your file into the space shown or click upload and choose your data file.<br>
                            <p><img src="{{ site.baseurl }}/assets/images/help/multiple-activities-2.png" class="img img-responsive center-block"><br></p>
                        </li>   
                        <li>
                            If your file contains multiple tabs, select the relevant one. The data will be previewed below.<br>
                            <p><img src="{{ site.baseurl }}/assets/images/help/multiple-activities-3.png" class="img img-responsive center-block"><br></p>
                        </li>   
                        <li>
                            If all mandatory fields which can't be mapped from your file, you can click ‘Save this sheet’. Your data is now registered to your project in AssayReg. <br>
                            <p><img src="{{ site.baseurl }}/assets/images/help/multiple-activities-4.png" class="img img-responsive center-block"><br></p>
                        </li>
                    </ul>
                </p>

                <h3 class="blue" >Data mapping</h3>
                <p>If you are uploading data from a file containing supplementary data, you may have to specify which columns in your file correspond to which Activity columns. This is especially important where there are <em>mandatory</em> fields for the specified Activity - that is to say, fields which cannot be empty for a single result.</p>

                <p>AssayReg uses data mapping to help with data integrity and also to allow conversion to formats required by public databases such as <a href="https://pubchem.ncbi.nlm.nih.gov/about.html" target="_blank">PubChem</a> and <a href="https://www.ebi.ac.uk/chembl/" target="_blank">ChEMBL</a>.</p>

                <h3 class="blue" >Auto mapping</h3>
                <p>AssayReg will attempt to "automap" your columns to the Activity columns. Columns in your file with a matching column in the Activity have a green mapping icon <span class="glyphicon glyphicon-random text-success"></span> . Columns in your file which cannot be automapped have a red mapping icon <span class="glyphicon glyphicon-random text-danger"></span> .</p>

                <p>You will need to map a column in your file to an Activity column manually if the names are slightly different - for example, you may have a column called "1st Run" in your file and a column called "1st Observation" in the Activity table. They have the same meaning for your work but have been labelled differently. To do this, click the mapping icon in the column you want to map.<br>
                </p>
                <p><img src="{{ site.baseurl }}/assets/images/help/filter-icon.png" class="img img-responsive center-block"><br></p>
                <p>A window wil display which will allow you to specify the field you wish to map to.</p>
                <p><img src="{{ site.baseurl }}/assets/images/help/mapping-popup.png" class="img img-responsive center-block"><br></p>

                <h3 class="blue" >Unmappable fields</h3>
                <p>Unmappable fields are caused by data fields in your file not matching the type expected by AssayReg for the Assay you are adding to. For example, you may be mapping your column containing text descriptions to a column expecting numerical values or dates.</p> 

                <p>Unmappable fields are shown in the mapping popup window for a particular column. You will see a message stating that there is a data type conflict, and the rows causing the issue (together with the row value) are displayed in a table.</p>
                <p><img src="{{ site.baseurl }}/assets/images/help/unmappable-fields.png" class="img img-responsive center-block"></p>

                <p>If this happens you should correct the data in your Excel file, and try uploading again. If you believe your data to be in the correct format, you should contact an AssayReg administrator. <a href="mailto:info@chembiohub.ox.ac.uk" role="button" class="btn btn-default"><span class="glyphicon glyphicon-envelope"></span> info@chembiohub.ox.ac.uk</a></p>

                <h3 class="blue" >Save</h3>
                <p>Once all of your fields are mapped, you are able to click <strong>Save This Sheet</strong>. Your data will be saved, and will be visible in the activities table.</p>

                <h2 class="blue" id="searching">Search page</h2>
                <p>AssayReg allows you to search for data across Projects, Sub-Projects and Assays via the Search Page. You can also carry out text searches via the search bar at the top of every page (including this one).</p>

                <p>The search bar allows you to type text, with matches for that text displayed instantly below. If the text matches any value in  Assay, Sub-Project or Project titles, you can click those links and see data for that item in the search page.</p>

                <p><img src="{{ site.baseurl }}/assets/images/help/searchbar.png" class="img img-responsive center-block"></p>

                <p>You are also able to search for your text phrase easily on <a href="https://pubchem.ncbi.nlm.nih.gov/about.html" target="_blank">PubChem</a> - just click the link at the bottom, a new window or tab will open in your browser and you will see results for your search displayed on the PubChem website.</p>

                <p>The search results page is shown when you click the <strong>Go</strong> button next to the search bar or select an option below the search bar.</p>

                <h3 class="blue" >Filters</h3>
                <p>The Search Page allows you to filter the results shown in a number of ways. Whenever a filter is used, the results are updated automatically. To remove all selections you've made for a single filter, click <strong>Clear</strong> underneath the box.</p>

                <h3 class="blue" >Dates</h3>
                <p>You can specify a date range for when records were added to the system - use the <strong>Activity Date From</strong> and <strong>Activity Date To</strong> calendar fields to specify your dates. Results are updated automatically. To remove a date selection, open the date popup and click Clear.</p>
                <p><img src="{{ site.baseurl }}/assets/images/help/date-popup.png" class="img img-responsive center-block"></p>

                <h3 class="blue" >User</h3>
                <p>You can specify the user or users who uploaded the data you wish to see. Select the names of users from the dropdown list, and they will be displayed as a tag list in the search box. You can remove any users you have selected. Results are updated automatically.</p>

                <h3 class="blue" >Project / Sub-Project / Assay filtering</h3>
                <p>You can specify the Project, Sub-Project or Assay the results belong to using the appropriate search fields. Pick the names of the Project/Sub-Project/Assay you want to narrow results down by from the dropdown list, and they are displayed as a tag list in the search box. You can remove items as you need to. Results are updated automatically.</p>

                <h3 class="blue" >Text filtering</h3>
                <p>At the top of the Results table section, there is a text box which allows you to filter the Activities based on text entered here. So for example, if you type "dichloro" into the text box, the Activities table will only show rows that contain "dichloro" in any of the columns, in addition to any other filters you have applied via the search form.</p>

                <h2 class="blue" id="chembl">Depositing data to ChEMBL</h2>
                <p>
                    <ul>
                        <li>AssayReg translates your data to the format required by <a href="https://www.ebi.ac.uk/chembl/" target="_blank">ChEMBL</a>. To view data in a ChEMBL format, use the Search page to find your data.</li>
                        <li>
                            You are now in the AssayReg search page. On the data record you wish to export, click ‘View as ChEMBL data’
                            <p><img src="{{ site.baseurl }}/assets/images/help/chembl-1.png" class="img img-responsive center-block"></p>
                        </li>
                        <li>
                            Your activity data should now be visible as a JSON schema form. This is the format in which it will be deposited to ChEMBL - highlight the text, copy and paste into the ChEMBL submission form.
                            <p><img src="{{ site.baseurl }}/assets/images/help/chembl-2.png" class="img img-responsive center-block"></p>
                        </li>
                    </ul>
                </p>


            </div>
        </div>

    </div>

</div>

<div ng-include="'views/help-chemireg.html'"></div>

<div class="spacer"></div>

<div class="row mt">
    <div class="col-sm-8 col-sm-offset-2">
        <h2 class="blue" id="chemireg-section">ChemiReg Help section<br><small>How-tos, information and FAQs</small></h2>   
    </div>

</div>

<div class="row">
    <div class="col-sm-8 col-sm-offset-2">
        <h2 class="subheading">File Submission - What ChemiReg can and can’t accept currently</h2>
    </div>

    <div class="col-sm-5 col-sm-offset-2">

        <div class="row">
            

            <div class="col-xs-12">
                <h2 class="blue"><span class="glyphicon glyphicon-ok-circle" style="color:#3c763d;"></span> ChemiReg can accept Excel .XLSX files (newer Office versions)</h2>
            </div>

            <div class="col-xs-12">
                <div class="well">
                    <p class="nexa">The file must contain column headers in the top row, with all data organised in the relevant columns underneath. Figures and images cannot currently be accepted.</p>

                    <p class="nexa">The submitted Excel file may contain structural information.  In this case, use the dropdown menu to select the column heading which containing structural information (eg. SMILES). This will ensure a compound structure is drawn in the system following submission.</p>

                    <p class="nexa">An Excel file may be submitted containing no structural information. In this case submit the file as the default “No structural information” using the available dropdown menu. This will assign each record with a unique ID as normal but with no structure information.</p>

                    <p class="nexa"><a role="button" class="btn btn-default" href="/files/faq/example-excel-file-with-structures.xlsx"><span class="glyphicon glyphicon-floppy-disk"></span> Download</a> an example of an Excel file that could be registered in the system containing structural information.</strong> </p>

                    <p class="nexa"> <a role="button" class="btn btn-default" href="/files/faq/example-excel-file-without-structures.xlsx"><span class="glyphicon glyphicon-floppy-disk"></span> Download</a> an example of an Excel file that could be registered in the system containing NO structural information.</strong></p>
                </div>
            </div>

            <div class="col-xs-12">
                <h2 class="blue"><span class="glyphicon glyphicon-ok-circle"  style="color:#3c763d;"></span> ChemiReg can accept .SDF files</h2>
            </div>

            <div class="col-xs-12">
                <div class="well">
                    <p class="nexa">Most SDF files can be uploaded without issue.</p>

                    <p class="nexa"><a role="button" class="btn btn-default" href="/files/faq/example-SDF-file.sdf"><span class="glyphicon glyphicon-floppy-disk"></span> Download</a> an example of an SDF file that could be registered in the system</p>
                </div>

                
            </div>

            <div class="col-xs-12">
                <h2 class="blue"><span class="glyphicon glyphicon-ok-circle" style="color:#3c763d;"></span> ChemiReg can accept ChemDraw data when saved in SDF format</h2>
            </div>

            <div class="col-xs-12">
                <div class="well">
                    <p class="nexa"><em>To find out how to format your ChemDraw files to be saved to ChemiReg, please refer to the following help document.</em></p>
                
                    <!-- <p class="nexa">ChemDraw files should be drawn with no descriptive linkers or arrows between molecules. Note that any entity in a file that is not explicitly bonded to another compound will also be registered as a separate entity. </p>
    
                    <p class="nexa"><a role="button" class="btn btn-default" href="/files/faq/example-ChemDraw-file-correct-format.cdx"><span class="glyphicon glyphicon-floppy-disk"></span> Download</a> an example of a CDXML file with <strong>compounds organised in the correct format </strong></p>
    
                    <p class="nexa"><a role="button" class="btn btn-default" href="/files/faq/example-ChemDraw-file-Incorrect-Format.cdx"><span class="glyphicon glyphicon-floppy-disk"></span> Download</a> an example of a CDXML file with <strong>compounds NOT organised in the correct format </strong></p>
    
                    <p class="nexa">If you wish for associated structures that are not bonded to be registered as the same entity (such as a salt) please follow these steps:<br>
                        <ol style="font-family:NexaLight">
                            <li class="nexa">In ChemDraw, please group the associated molecules using “Ctrl+G” or the equivalent Mac command</li>
                            <li class="nexa">Save the ChemDraw file as an SDF</li>
                            <li class="nexa">Upload the SDF file into ChemiReg as normal. Note that you can still submit multiple compounds, (grouped or not) in the same file by following this process.</li>
                        </ol>
                    </p>
    
                    <p class="nexa">Here are examples of a <strong>grouped compound (a salt) in a ChemDraw file</strong>, and the associated SDF that could be registered in the system.<br> <a role="button" class="btn btn-default" href="/files/faq/example-salt.cdx"><span class="glyphicon glyphicon-floppy-disk"></span> Download ChemDraw file</a> <a role="button" class="btn btn-default" href="/files/faq/examplesalt.sdf"><span class="glyphicon glyphicon-floppy-disk"></span> Download SDF file</a></p> -->
                </div>

            </div>

        </div>

    </div>



    <div class="col-sm-3">

        <div class="row">
            <div class="col-xs-12">
                <h2 class="blue"><span class="glyphicon glyphicon-remove-circle"  style="color:#a94442"></span> What ChemiReg can’t do (yet):</h2>
            </div>

            <div class="col-xs-12">
                <div class="well">
                    <p class="nexa">ChemiReg can’t register compounds containing R-groups.</p>
    
                    <p class="nexa">ChemiReg cannot currently register files containing images e.g. spectra data. This does not include structural information e.g. .SDF file structures are fine).</p>
    
                    <p class="nexa">Reaction pathways cannot currently be accepted.</p>
                </div>
            </div>
        </div>

    </div>



    

    



</div>

<!-- <div class="row">

    <div class="col-xs-12">
        <h2 class="subheading">FAQs</h2>
    </div>
    <div class="col-xs-12">
        <h2 class="blue">Why do some of the projects I can see have the "Add Compounds" or "Add Items" button greyed out?</h2>
        <p class="nexa">A greyed-out "Add Compounds" or "Add Items" button indicates that while you can view compounds or items for a particular project, you cannot add compounds or items to that project. This is a security setting within ChemiReg.<br>If you believe you should be able to add compounds or items to the specified project, please contact an administrator or a member of the ChemBio Hub team to change your permissions.</p>

    </div>

</div> -->
<div class="row">

<div class="col-sm-8 col-sm-offset-2">
    <h2 class="subheading">Archiving and restoring items and compounds</h2>
</div>
<div class="col-sm-8 col-sm-offset-2">
    <h2 class="blue">Can I archive items in my project which are no longer relevant or were added in error?</h2>

    <p class="nexa"><strong>Yes</strong>.  To archive an item or items, on the Search Results page, select the Edit button at the top of the results grid.  The first column will now contain an Archive/Restore button. Click this on any items you wish to archive.</p>

    <h2 class="blue">Can I restore previously archived items in my project?</h2>

    <p class="nexa"><strong>Yes</strong>.  To restore an item or items, on the Search Results page, select the Edit button at the top of the results grid.  Now select the filter option in the first column header to "show only archived".  Click on any items you wish to restore.</p>
</div>
</div>

<div class="row">
    <div class="col-sm-8 col-sm-offset-2">
        <h2 class="subheading">Supported Browsers</h2>
    </div>
    <div class="col-sm-8 col-sm-offset-2 text-center">
        <img src="images/accepted-browsers.png">
    </div>
</div>


<!-- Maybe only have this on any demo versions we have - or make the test instances have exactly the same teest data so that these example searches work? -->
<!-- <div class="row">
    
    <div class="col-xs-12">
        <h2 class="subheading">Example Searches<br><small style="color:white">These links will take you direct to the search page with the appropriate results</small></h2>
    </div>

    <div class="col-xs-11 col-xs-offset-1">
        <ul class="list-unstyled">
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?related_molregno__chembl__chembl_id__in=UOXQT26KMZ,UOXSU43EQV&limit=&offset=" > Show me the items with System Ids UOXSU43EQV or UOXQT26KMZ <span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?search_custom_fields__kv_any=Custom%20Identifier%7CLB1h&limit=&offset=" > Show me the item with user custom ID LB1h<span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?search_custom_fields__kv_any=Shelf%20Location%7CFreezerA&limit=&offset=" > Show me the items kept in Freezer A <span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?search_custom_fields__kv_any=Storage%20Conditions%7CRoom%20Temp.&limit=&offset=" > Show me the items stored at room temperature <span class="glyphicon glyphicon-new-window"></span></a></h3></li>

            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?project=admin&functional_group=W09YMV09Q04&limit=&offset=" > Show me the carbonyls with nitrogen <span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/searchsearch_custom_fields__kv_any=Spectroscopy%20Checklist%7CHDMS,Spectroscopy%20Checklist%7CC13%20nmr,Spectroscopy%20Checklist%7CH1%20nmr&limit=&offset=" > Show me compounds that are fully characterised with NMR and HDMS <span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?with_substructure=Molecule%20from%20ChemDoodle%20Web%20Components%0A%0Ahttp:%2F%2Fwww.ichemlabs.com%0A%20%205%20%205%20%200%20%200%20%200%20%200%20%20%20%20%20%20%20%20%20%20%20%20999%20V2000%0A%20%20%20%200.0000%20%20%20%200.7694%20%20%20%200.0000%20O%20%20%200%20%200%20%200%20%200%20%200%20%200%0A%20%20%20%200.8090%20%20%20%200.1816%20%20%20%200.0000%20C%20%20%200%20%200%20%200%20%200%20%200%20%200%0A%20%20%20%200.5000%20%20%20-0.7694%20%20%20%200.0000%20C%20%20%200%20%200%20%200%20%200%20%200%20%200%0A%20%20%20-0.5000%20%20%20-0.7694%20%20%20%200.0000%20C%20%20%200%20%200%20%200%20%200%20%200%20%200%0A%20%20%20-0.8090%20%20%20%200.1816%20%20%20%200.0000%20N%20%20%200%20%200%20%200%20%200%20%200%20%200%0A%20%201%20%2021%20%200%20%20%20%20%200%20%200%0A%20%202%20%2032%20%200%20%20%20%20%200%20%200%0A%20%203%20%2041%20%200%20%20%20%20%200%20%200%0A%20%204%20%2052%20%200%20%20%20%20%200%20%200%0A%20%205%20%2011%20%200%20%20%20%20%200%20%200%0AM%20%20END&limit=&offset=" > Show me compounds that have an isoxazole scaffold <span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            <li><h3 class="blue"> <a ng-href="{{cbh.prefix}}/#/search?created__gte=2015-05-13&created__lte=2015-06-04" > Show me compounds registered between 13 May and 4th June 2015 <span class="glyphicon glyphicon-new-window"></span></a></h3></li>
            

        </ul>
    </div>

    
    
    

</div> -->
<div class="spacer"></div>



