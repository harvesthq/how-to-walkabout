All of the companies participating in the Walkabout are stored in company.php. Within that file, each company is an instance of a simple class that gets added to a big group array.

Like this:


    $companies[] = new walk_company("pc-harvest","Harvest","http://www.getharvest.com", "187 Lafayette St, 6th Fl", "Soho", "40.720786,-73.998427", "12pm-6pm", "Harvest builds powerful web-based software for time tracking and invoicing. Relied on by businesses in over 100 countries, Harvest makes it faster and easier to track time and invoice clients.", "Use the elevator outside to your right.");


The parameters for the class initialization are:

- slug (used for tying companies to images and for URLs in the mobile version)
- name
- url
- address
- neighborhood (the mobile site breaks companies down by neighborhood for quicker navigation)
- latlong (formatted as "40.72436,-73.99746")
- hours (that they are participating in the walkabout)
- description (short company description)
- details (any special details specific to walkabout)