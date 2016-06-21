---
layout: page
root: ..
title: Use
published: true
---

These pages contain information on how to 
use {{ site.software_name }} i.e. contain our current adapted end-user documentation.

## Using ShowYourWorking

((TODO separate out generic-use user steps from chemireg-specific usage steps))

((TODO current user help docs are now out of date - much search functionality has changed. Needs rewriting in a generic way for ShowYourWorking. Altered functionality and screenshots to be accounted for ))

<div class="row mt">
    <div class="col-sm-8 col-sm-offset-2"  style="padding-left:15px;">
        
        <a name="top" href="#chemireg-section"><h2 class="blue" id="top">ChemBio Hub platform Help section<br><small>How-tos, information and FAQs</small></h2> </a>
                          
    </div>

</div>



<div class="row">
    <div class="col-sm-8 col-sm-offset-2" data-spy="scroll" style="position: relative;">

        <div class="row">
            <div class="col-xs-12">
                <div class="well text-center">
                    <em>Jump to</em>: 
                    <a href="#setup"><strong class="nexa">Set up a new project</strong></a> | 
                    <a href="#adding-users"><strong class="nexa">Add users</strong></a> | 
                    <a href="#adding-data"><strong class="nexa">Put your data into a project</strong></a> | 
                    <a href="#attachments"><strong class="nexa">Attach extra files</strong></a> | <br>
                    <a href="#search"><strong class="nexa">Search your data</strong></a> | 
                    <a href="#chem-search"><strong class="nexa">Chemical searching</strong></a> | 
                    <a href="#edit-data"><strong class="nexa">Edit your data</strong></a> | 
                    <a href="#export-data"><strong class="nexa">Export your data</strong></a> | 
                </div>
                
                
                <p><h2 class="blue" id="problem">What to do if you have a problem</h2></p>
             
If you encounter a problem with ChemiReg, and this help document does not provide the answer please use the menu box to submit an issue - click the ChemiReg logo and select <em>Report an Issue</em>.  Alternatively please [Get in Touch](http://showyourworking.github.io/project/HelpAndSupport.html) 




<a name="setup"><h2 class="blue" id="setup">Set up a new project</h2></a>
                <p>When you first log in to ChemBio Hub, you are shown a list of projects. If you're using the system for the first time, this may be an empty list, so you'll have to add a project. To do this, click the <strong class="blue nexa">Add Project</strong> button. You'll be shown a popup window where you can specify a title for your project, the type of project it is, whether you want it to start an incremental counter field and also project data fields.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/add-project.png"></p>

                

                <p>The project data fields are part of what makes ChemBio Hub so useful - these are columns in your data that you can make mandatory for people adding data, have text, numeric, multiple choice, tagging or even file attachment fields. Fill in the parts of the field as required. If you want to add more, click the <strong class="blue nexa">Add</strong> button. When you're done, click <strong class="blue nexa">Save Changes and Close</strong>.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/new-project.png"></p>

                <p>The page will reload and you'll see your new project at the top of the list.</p>

                <a href="#top"><strong class="nexa">back to top</strong></a>
                                
                <a name="adding-users"><h2 class="blue" id="adding-users">Add users</h2></a>

                               <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/project-summary.png"></p>


                <p>Now you have your project set up how you want it, you are the project owner and can do things like add more fields, and change whether fields are mandatory. Another important thing you can do is to add users to your project. You can do this by clicking on the <strong class="blue nexa">Edit User Roles</strong> link on your project.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/user-roles.png"></p>

               In the popup window, you can add users to your project with different roles:
               
               
               <p><strong>Owners</strong> can edit everything about the project and add other users.
               <p><strong>Editors</strong> can edit and view data which has been added but nothing else. 
               <p><strong>Viewers</strong> can only see the data for that project.</p>
               
                <p>Type the name of the user you want to assign a role to and click their name in the list.

                <p>You can invite people to log into the system once you have added a project. Open the main menu button in the top right corner and click <strong class="blue nexa">Send an invitation.</strong></p>

            	<a href="#top"><strong class="nexa">back to top</strong></a>
                    
                <a name="adding-data"><h2 class="blue" id="adding-data">Put your data into a project</h2></a>
                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/project-summary.png"></p>


                <p>Once you've set up your project and users, you can start adding data either one item at a time or as a dataset in an Excel file. Chemical data can also be added via SDF files. If you need to know which project data fields are in your project, you can download a template file with the headers in. Choose your file and click <strong class="blue nexa">Upload</strong>.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/upload-data.png"></p>

                <p>When adding data to a project, your column headers in your file might not exactly match the ones in the project, or you might have extra fields that you want to also add or just ignore. If your data column can be "automapped" to a project column, it wil have a green label in the header. If a column has not been automapped, you can either upload it as it is and create a new column, or you can manually map it to a project column. To do this click the icon in the column header. You will see a list of available project fields to map to. Pick one from the list and it will show as a green mapped column in the table header.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/data-mapping.png"></p>

                <p>When you're done, click <strong class="blue nexa">Save these Records</strong>. You are then forwarded to the search page so that you can see your uploaded results. Data which has come from one file is given an upload ID so that you can see which records came from the same file later on.</p>

                <a href="#top"><strong class="nexa">back to top</strong></a>

                <a name="search"><h2 class="blue" id="search">Search your data</h2></a>
                
                <p>Once you've added some data, you'll probably want to refer back to it at some point in the future! ChemBio Hub has a powerful search architecture. You can do simple text searches - start typing in the Search ChemBio Hub platform box.</p>

                <p>You can do more complex searches and filter by individual field. Click the button in the column header and chose the type of filter you want for that column. All column filters and sorts are shown in the boxes above the results table. You can remove a search filter by clicking the close x in the top right corner of each.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/search-filter.png"></p>

                <p>If you find you're doing a particular search over and over - for example "data added within the last two weeks" - you can save your search to re-run later. Open the <strong class="blue nexa">Saved search</strong> menu and click <strong class="blue nexa">Save this search</strong>. Give your search a title to refer to later and click <strong class="blue nexa">Save Changes and Close</strong>. To re-run your search, click My saved searches in the Saved search menu. You can run the search parameters again and get new results or you can re-run the search with the same results returned as it was when you saved that search and only see results from that time.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/saved-search.png"></p>

                <p class="text-right"><a href="#top"><strong class="nexa">back to top</strong></a></p>

				<a name="chem-search"><h2 class="blue" id="chem-search">Chemical searching</h2></a> 
                
                <p>If your system is set up to hold chemical data and you have at least one chemical project set up, you can search for compounds based on chemical similarity. To launch the chemical search form, click the button in the Structure column header. This will show a chemical sketcher and a choice of Substructure and Exact Match searches.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/data-mapping.png"></p>

                <p>You can use the Saved Searches feature with chemical search to save repeatedly sketching the same molecule.</p>

                <p class="text-right"><a href="#top"><strong class="nexa">back to top</strong></a></p>


                <a name="edit-data"><h2 class="blue" id="edit-data">Edit your data</h2></a>
                 
                <p></p>
                If you need to modify or add extra fields to your data, you can do so in a couple of ways:

                <ul>
                    <li><em>Edit one record</em> - open the details popup window for that record by clicking the system ID number and then clicking Edit.</li>
                    <li><em>Bulk edit multiple records</em> - you can do drag-to-fill editing for multiple records. Make sure the data to be edited is all in the same project and that project is selected in the search form. You should now see an Edit button link above the table - click it and you can now edit data directly within the table. When you're done, the data will be automatically saved. To make more changes, click Edit again.</li>
                </ul>

                <p class="text-right"><a href="#top"><strong class="nexa">back to top</strong></a></p>

                <a name="attachments"><h2 class="blue" id="attachments">Attach extra files</h2></a>
             
                <p>One of the field types for the project fields that you set up at the start was File Upload. This means that you can attach extra files (like pictures, PowerPoint files, PDFs and more) to a data record. Make sure one of your project fields is a File Upload field, go to the record you want to attach a file to and click Edit.</p>

                <p class="text-center"><img src="img img-responsive img-thumbnail" src="/assets/images/help/add-attachments.png"></p>

                <p>Click the grey <strong class="blue nexa">+</strong> icon to choose a file to add. It will be uploaded automatically. To remove a file, click the x in the top right corner of the thumbnail. When you're done, click <strong class="blue nexa">Update Project data</strong> to save your record.</p>

                <p class="text-right"><a href="#top"><strong class="nexa">back to top</strong></a></p>

                <a name="export-data"><h2 class="blue" id="export-datas">Export your data</h2></a>
               
                <p>If you want to export your data in an Excel file, you can do so on the search page. Pick your search parameters and when you're ready, choose <strong class="blue nexa">Export all to Excel</strong> from the Export menu. If you have any Chemistry projects, you can also <strong class="blue nexa">Export all to SDF</strong>.</p>


<div ng-include="'views/help-chemireg.html'"></div>

<div class="spacer"></div>

<div class="row mt">
    <div class="col-sm-8 col-sm-offset-2">
        <a><h2 class="blue" id="chemireg-section">ChemiReg Help section<br><small>How-tos, information and FAQs</small></h2>  </a> 
               
        
    </div>

</div>

<div class="row">
    <div class="col-sm-8 col-sm-offset-2">
        <h2 class="subheading"><small>File Submission - What ChemiReg can and can’t accept currently</small></h2>
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
        <img src="/assets/images/accepted-browsers.png">
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
