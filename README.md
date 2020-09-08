# dataAna
Concept:
Component: the devices which contains by a product. For example you can define speaker, shell, screen for a phone device. The component include manufacturer, contact, failure rate, component name and id.
Fail Mode: the failure tested out by a tester(Audio Degradation, Hardware Degradation, Battery Degration etc.). the fail mode include fail mode name and id 
Mapping: a describe for a failure relation between component and fail mode.
Fail code: the code assigned to mapping, required 6 letters string

Requirement:
-Create and design DB table base on concept and insert basic data
-Create RESTAPIs:
     -Create component
     -List components
     -Create fail mode
     -List fail mode
     -Create mapping 
     -Remove mapping
     -Update mapping
     -List mapping
-Front-end side using API to create page which allow user to:
     -Page 1
        View component/fail mode table
        Able to create component/fail
     -Page 2
        View mapping table
        Modified mapping
        Remove mapping
        Update mapping

-Create dashboard page.
     -Show to the user 3 reports(you can define how to show to the user no matter charts, table…):
     -Top 5 of the most bad quality components.(highest fail rate)
     -Top 5 of the most used of test devices.(most appeared in mapping table)
     -Top 3 of the highest PFR(product failure rate) manufactory. (average fail rate of all components from one manufacturer)
     -Given at least 2 advice to the user.
     -Auto email to notice the manufactory about the failure details.
