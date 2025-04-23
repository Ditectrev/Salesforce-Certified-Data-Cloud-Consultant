# Salesforce Certified `Data Cloud` Consultant

### What does the Source Sequence reconciliation rule do in `Identity Resolution`?

- [ ] Includes data from sources where the data is most frequently occurring.
- [ ] Identifies which individual records should be merged into a unified profile by setting a priority for specific data sources.
- [ ] Identifies which data sources should be used in the process of reconcillation by prioritizing the most recently updated data sourc.
- [x] Sets the priority of specific data sources when building attributes in a unified profile, such as a
first or last name.

### Cumulus Financial uses `Data Cloud` to segment banking customers and activate them for direct mail via a Cloud File Storage activation. The company also wants to analyze individuals who have been in the segment within the last 2 years. Which `Data Cloud` component allows for this?

- [ ] Segment exclusion.
- [ ] Nested segments.
- [x] Segment membership Data Model Object.
- [ ] Calculated insights.

### How can a consultant modify attribute names to match a naming convention in Cloud File Storage targets?

- [ ] Use a formula field to update the field name in an activation.
- [ ] Update attribute names in the data stream configuration.
- [x] Set preferred attribute names when configuring activation.
- [ ] Update field names in the Data Model Object.

### A customer has a Master Customer table from their CRM to ingest into `Data Cloud`. The table contains a name and primary email address, along with other Personally Identifiable Information (PII). How should the fields be mapped to support `Identity Resolution`?

- [ ] Create a new custom object with fields that directly match the incoming table.
- [ ] Map all fields to the `Customer` object.
- [x] Map name to the `Individual` object and email address to the `Contact Point Email` object.
- [ ] Map all fields to the `Individual` object, adding a custom field for the email address.

### A customer wants to use the transactional data from their data warehouse in `Data Cloud`. They are only able to export the data via an `SFTP` site. How should the file be brought into `Data Cloud`?

- [x] Ingest the file with the `SFTP Connector`.
- [ ] Ingest the file through the `Cloud Storage Connector`.
- [ ] Manually import the file using the `Data Import Wizard`.
- [ ] Use Salesforce's `Data Loader` application to perform a bulk upload from a desktop.

### Cumulus Financial is currently using `Data Cloud` and ingesting transactional data from its backend system via an `S3 Connector` in `Upsert` mode. During the initial setup six months ago, the company created a formula field in `Data Cloud` to create a custom classification. It now needs to update this formula to account for more classifications. What should the consultant keep in mind with regard to formula field updates when using the `S3 Connector`?

- [ ] `Data Cloud` will initiate a `Full Refresh` of data from S3 and will update the formula on all records.
- [ ] `Data Cloud` will only update the formula on a go-forward basis for new records.
- [ ] `Data Cloud` does not support formula field updates for data streams of type `Upsert`.
- [x] `Data Cloud` will update the formula for all records at the next incremental `Upsert` refresh.

### Northern Trail Outfitters wants to implement `Data Cloud` and has several use cases in mind. Which two use cases are considered a good fit for `Data Cloud`?

- [x] To ingest and unify data from various sources to reconcile customer identity.
- [ ] To create and orchestrate cross-channel marketing messages.
- [x] To use harmonized data to more accurately understand the customer and business impact.
- [ ] To eliminate the need for separate business intelligence and IT data management tools.

### What should an organization use to stream inventory levels from an inventory management system into `Data Cloud` in a fast and scalable, near-real-time way?

- [ ] `Cloud Storage Connector`.
- [ ] `Commerce Cloud Connector`.
- [x] `Ingestion API`.
- [ ] `Marketing Cloud Personalization Connector`.

### A customer is trying to activate data from `Data Cloud` to an Amazon S3 Cloud File Storage Bucket. Which authentication type should the consultant recommend to connect to the S3 bucket from `Data Cloud`?

- [ ] Use a `S3 Private Key Certificate`.
- [ ] Use a `S3 Encrypted Username and Password`.
- [ ] Use a `JWT Token` generated on `S3`.
- [x] Use a `S3 Access Key` and `Secret Key`.

### Northern Trail Outfitters (NTO) wants to connect their B2C Commerce data with `Data Cloud` and bring two years of transactional history into `Data Cloud`. What should NTO use to achieve this?

- [ ] B2C Commerce Starter Bundles.
- [ ] `Direct Sales Order` entity ingestion.
- [ ] `Direct Sales Product` entity ingestion.
- [x] B2C Commerce Starter Bundles plus a custom extract.

### Cumulus Financial uses Service Cloud as its CRM and stores `Mobile Phone`, `Home Phone`, and `Work Phone` as three separate fields for its customers on the `Contact` record. The company plans to use `Data Cloud` and ingest the `Contact` object via the CRM Connector. What is the most efficient approach that a consultant should take when ingesting this data to ensure all the different phone numbers are properly mapped and available for use in activation?

- [ ] Ingest the `Contact` object and map the `Work Phone`, `Mobile Phone`, and `Home Phone` to the `Contact Point Phone` data map object from the Contact data stream.
- [x] Ingest the `Contact` object and use streaming transforms to normalize the phone numbers from the Contact data stream into a separate Phone data lake object (DLO) that contains three rows, and then map this new DLO to the `Contact Point Phone` data map object.
- [ ] Ingest the `Contact` object and then create a calculated insight to normalize the phone numbers, and then map to the `Contact Point Phone` data map object.
- [ ] Ingest the `Contact` object and create formula fields in the Contact data stream on the phone numbers, and then map to the `Contact Point Phone` data map object.

### To import campaign members into a campaign in Salesforce CRM, a user wants to export the segment to Amazon S3. The resulting file needs to include the Salesforce CRM Campaign ID in the name. What are two ways to achieve this outcome?

- [x] Include campaign identifier in the activation name.
- [ ] Hard code the campaign identifier as a new attribute in the campaign activation.
- [x] Include campaign identifier in the filename specification.
- [ ] Include campaign identifier in the segment name.

### A customer is concerned that the consolidation rate displayed in the `Identity Resolution` is quite low compared to their initial estimations. Which configuration change should a consultant consider in order to increase the consolidation rate?

- [ ] Change reconciliation rules to `Most Occurring`.
- [x] Increase the number of matching rules.
- [ ] Include additional attributes in the existing matching rules.
- [ ] Reduce the number of matching rules.

### A customer has a requirement to receive a notification whenever an activation fails for a particular segment. Which feature should the consultant use to solution for this use case?

- [ ] `Flow`.
- [ ] `Report`.
- [x] `Activation alert`.
- [ ] `Dashboard`.

### Which data model subject area defines the revenue or quantity for an opportunity by product family?

- [ ] `Engagement`.
- [ ] `Product`.
- [ ] `Party`.
- [x] `Sales Order`.

### When performing segmentation or activation, which time zone is used to publish and refresh data?

- [ ] Time zone specified on the activity at the time of creation.
- [ ] Time zone of the user creating the activity.
- [ ] Time zone of the `Data Cloud Admin` user.
- [x] Time zone set by the `Salesforce Data Cloud` org.

### Northern Trail Outfitters (NTO), an outdoor lifestyle clothing brand, recently started a new line of business. The new business specializes in gourmet camping food. For business reasons as well as security reasons, it's important to NTO to keep all `Data Cloud` data separated by brand. Which capability best supports NTO's desire to separate its data by brand?

- [ ] Data streams for each brand.
- [ ] Data Model Objects for each brand.
- [x] Data spaces for each brand.
- [ ] Data sources for each brand.

### A `Data Cloud` customer wants to adjust their `Identity Resolution` rules to increase their accuracy of matches. Rather than matching on email address, they want to review a rule that joins their CRM Contacts with their Marketing Contacts, where both use the `CRM ID` as their primary key. Which two steps should the consultant take to address this new use case?

- [x] Map the primary key from the two systems to `Party` Identification, using `CRM ID` as the identification name for both.
- [ ] Map the primary key from the two systems to `Party` Identification, using `CRM ID` as the identification name for individuals coming from the CRM, and `Marketing ID` as the identification name for individuals coming from the marketing platform.
- [ ] Create a custom matching rule for an exact match on the `Individual ID` attribute.
- [x] Create a matching rule based on party identification that matches on `CRM ID` as the party identification name.

### Cumulus Financial created a segment called `High Investment Balance Customers`. This is a foundational segment that includes several segmentation criteria the marketing team should consistently use. Which feature should the consultant suggest the marketing team use to ensure this consistency when creating future, more refined segments?

- [x] Create new segments using nested segments.
- [ ] Create a `High Investment Balance` calculated insight.
- [ ] Package `High Investment Balance Customers` in a data kit.
- [ ] Create new segments by cloning `High Investment Balance Customers`.

### What does it mean to build a trust-based, first-party data asset?

- [x] To provide transparency and security for data gathered from individuals who provide consent for its use and receive value in exchange.
- [ ] To provide trusted, first-party data in the `Data Cloud` Marketplace that follows all compliance regulations.
- [ ] To ensure opt-in consents are collected for all email marketing as required by law.
- [ ] To obtain competitive data from reliable sources through interviews, surveys, and polls.

### Which two dependencies prevent a data stream from being deleted?

- [x] The underlying data lake object is mapped to a Data Model Object.
- [x] The underlying data lake object is used in a data transform.
- [ ] The underlying data lake object is used in activation.
- [ ] The underlying data lake object is used in segmentation.

### What is `Data Cloud`'s primary value to customers?

- [x] To provide a unified view of a customer and their related data.
- [ ] To connect all systems with a golden record.
- [ ] To create a single source of truth for all anonymous data.
- [ ] To create personalized campaigns by listening, understanding, and acting on customer behavior.

### Which consideration related to the way `Data Cloud` ingests CRM data is true?

- [ ] CRM data cannot be manually refreshed and must wait for the next scheduled synchronization.
- [ ] The CRM Connector's synchronization times can be customized to up to 15-minute intervals.
- [ ] Formula fields are refreshed at regular sync intervals and are updated at the next `Full Refresh`.
- [x] The CRM Connector allows standard fields to stream into `Data Cloud` in real time.

### During a privacy law discussion with a customer, the customer indicates they need to honor requests for the `Right to be Forgotten`. The consultant determines that Consent API will solve this business need. Which two considerations should the consultant inform the customer about?

- [x] Data deletion requests are reprocessed at 30, 60, and 90 days.
- [ ] Data deletion requests are processed within 1 hour.
- [x] Data deletion requests are submitted for `Individual` profiles.
- [ ] Data deletion requests submitted to `Data Cloud` are passed to all connected Salesforce clouds.

### Which permission setting should a consultant check if the custom Salesforce CRM object is not available in New Data Stream configuration?

- [ ] Confirm the `Create` object permission is enabled in the `Data Cloud` org.
- [x] Confirm the `View All` object permission is enabled in the source `Salesforce CRM` org.
- [ ] Confirm the `Ingest` Object permission is enabled in the `Salesforce CRM` org.
- [ ] Confirm that the `Modify` Object permission is enabled in the `Data Cloud` org.

### Where is value suggestion for attributes in segmentation enabled when creating the DMO?

- [ ] Data Mapping.
- [ ] Data Transformation.
- [x] Segment Setup.
- [ ] Data Stream Setup.

### Which two steps should a consultant take if a successfully configured Amazon S3 data stream fails to refresh with a `NO FILE FOUND` error message?

- [x] Check if the file exists in the specified bucket location.
- [x] Check if correct permissions are configured for the `Data Cloud` user.
- [ ] Check if the Amazon S3 data source is enabled in `Data Cloud` setup.
- [ ] Check if correct permissions are configured for the S3 user.

### What is the result of a segmentation criteria filtering on `City | Is Equal To | 'San José'`?

- [ ] Cities containing `San José`, `San Jose`, `san jose`, or `san jose`.
- [ ] Cities only containing `San Jose` or `san jose`.
- [ ] Cities only containing `San Jose` or `San Jose`.
- [x] Cities only containing `San José` or `san josé`.

### Northern Trail Outfitters wants to use some of its `Marketing Cloud data` in `Data Cloud`. Which engagement channel data will require custom integration?

- [ ] `SMS`.
- [ ] `Email`.
- [x] `CloudPage`.
- [ ] `Mobile push`.

### What should a user do to pause a segment activation with the intent of using that segment again?

- [ ] Deactivate the segment.
- [ ] Delete the segment.
- [ ] Skip the activation.
- [x] Stop the publish schedule.

### Which configuration supports separate Amazon S3 buckets for data ingestion and activation?

- [x] Dedicated S3 data sources in `Data Cloud` setup.
- [ ] Multiple S3 connectors in `Data Cloud` setup.
- [ ] Dedicated S3 data sources in `Activation` setup.
- [ ] Separate user credentials for data stream and `Activation` target.

### Luxury Retailers created a segment targeting high value customers that it activates through Marketing Cloud for email communication. The company notices that the activated count is smaller than the segment count. What is a reason for this?

- [ ] Marketing Cloud activations apply a frequency cap and limit the number of records that can be sent in an activation.
- [x] `Data Cloud` enforces the presence of `Contact Point for Marketing Cloud` activations. If the individual does not have a related Contact Point, it will not be activated.
- [ ] Marketing Cloud activations automatically suppress individuals who are unengaged and have not opened or clicked on an email in the last six months.
- [ ] Marketing Cloud activations only activate those individuals that already exist in Marketing Cloud.
They do not allow activation of new records.

### When creating a segment on an individual, what is the result of using two separate containers linked by an AND as shown below? `GoodsProduct | Count | At Least | 1 Color | Is Equal To | red AND GoodsProduct | Count | At Least | 1 PrimaryProductCategory | Is Equal To | shoes`

- [x] Individuals who purchased at least one of any `red` product and also purchased at least one pair of `shoes`.
- [ ] Individuals who purchased at least one `red shoes` as a single line item in a purchase.
- [ ] Individuals who made a purchase of at least one `red shoes` and nothing else.
- [ ] Individuals who purchased at least one of any `red` product or purchased at least one pair of `shoes`.

### Cloud Kicks received a `Request to be Forgotten` by a customer. In which two ways should a consultant use `Data Cloud` to honor this request?

- [ ] Delete the data from the incoming data stream and perform a `Full Refresh`.
- [x] Add the `Individual ID` to a headerless file and use the delete from file functionality.
- [ ] Use `Data Explorer` to locate and manually remove the `Individual`.
- [x] Use the Consent API to suppress processing and delete the `Individual` and related records from source data streams.

### A retailer wants to unify profiles using Loyalty ID which is different than the unique ID of their customers. Which object should the consultant use in `Identity Resolution` to perform exact match rules on the Loyalty ID?

- [x] `Party Identification` object.
- [ ] `Loyalty Identification` object.
- [ ] `Individual` object.
- [ ] `Contact Identification` object.

### A consultant has an activation that is set to publish every 12 hours, but has discovered that updates to the data prior to activation are delayed by up to 24 hours. Which two areas should a consultant review to troubleshoot this issue?

- [ ] Review data transformations to ensure they're run after calculated insights.
- [ ] Review calculated insights to make sure they're run after the segments are refreshed.
- [x] Review segments to ensure they're refreshed after the data is ingested.
- [x] Review calculated insights to make sure they're run before segments are refreshed.

### Cumulus Financial wants to segregate Salesforce CRM Account data based on `Country` for its `Data Cloud` users. What should the consultant do to accomplish this?

- [ ] Use Salesforce sharing rules on the `Account` object to filter and segregate records based on `Country`.
- [ ] Use formula fields based on the `Account Country` field to filter incoming records.
- [ ] Use streaming transforms to filter out `Account` data based on `Country` and map to separate Data Model Objects accordingly.
- [x] Use the data spaces feature and apply filtering on the `Account` data lake object based on `Country`.

### A customer notices that their consolidation rate has recently increased. They contact the consultant to ask why. What are two likely explanations for the increase?

- [x] New data sources have been added to `Data Cloud` that largely overlap with the existing profiles.
- [x] `Identity Resolution` rules have been added to the ruleset to increase the number of matched profiles.
- [ ] Duplicates have been removed from source system data streams.
- [ ] `Identity Resolution` rules have been removed to reduce the number of matched profiles.

### `Data Cloud` consultant recently discovered that their `Identity Resolution` process is matching individuals that share email addresses or phone numbers, but are not actually the same individual. What should the consultant do to address this issue?

- [ ] Modify the existing ruleset to use fewer matching rules, run the ruleset and review the updated results, then adjust as needed until the individuals are matching correctly.
- [x] Create and run a new ruleset with stricter matching criteria, compare the two rulesets to review and verify the results, and then migrate to the new ruleset once approved.
- [ ] Create and run a new ruleset with fewer matching rules, compare the two rulesets to review and verify the results, and then migrate to the new ruleset once approved.
- [ ] Modify the existing ruleset with stricter matching criteria, run the ruleset and review the updated results, then adjust as needed until the individuals are matching correctly.

### `Data Cloud` receives a nightly file of all ecommerce transactions from the previous day. Several segments and activations depend upon calculated insights from the updated data in order to maintain accuracy in the customer's scheduled campaign messages. What should the consultant do to ensure the ecommerce data is ready for use for each of the scheduled activations?

- [ ] Ensure the activations are set to `Incremental Activation` and automatically publish every hour.
- [x] Use `Flow` to trigger a change data event on the ecommerce data to refresh calculated insights and segments before the activations are scheduled to run.
- [ ] Set a refresh schedule for the calculated insights to occur every hour.
- [ ] Ensure the segments are set to `Rapid Publish` and set to refresh every hour.

### A client wants to bring in loyalty data from a custom object in Salesforce CRM that contains a point balance for accrued hotel points and airline points within the same record. The client wants to split these point systems into two separate records for better tracking and processing. What should a consultant recommend in this scenario?

- [x] Use batch transforms to create a second data lake object.
- [ ] Create a junction object in Salesforce CRM and modify the ingestion strategy.
- [ ] Clone the data source object.
- [ ] Create a data kit from the data lake object and deploy it to the same `Data Cloud` org.

### Which operator should a consultant use to create a segment for a birthday campaign that is evaluated daily?

- [ ] `Is Today`.
- [ ] `Is Birthday`.
- [ ] `Is Between`.
- [x] `Is Anniversary Of`.

### A new user of `Data Cloud` only needs to be able to review individual rows of ingested data and validate that it has been modeled successfully to its linked Data Model Object. The user will also need to make changes if required. What is the minimum permission set needed to accommodate this use case?

- [ ] `Data Cloud` for `Marketing Specialist`.
- [ ] `Data Cloud Admin`.
- [x] `Data Cloud` for `Marketing Data Aware Specialist`.
- [ ] `Data Cloud User`.

### A consultant is discussing the benefits of `Data Cloud` with a customer that has multiple disjointed data sources. Which two functional areas should the consultant highlight in relation to managing customer data?

- [x] Unified Profiles.
- [x] Data Harmonization.
- [ ] Master Data Management.
- [ ] Data Marketplace.

### Northern Trail Outfitters is using the `Marketing Cloud Starter Data Bundles` to bring `Marketing Cloud` data into `Data Cloud`. What are two of the available datasets in `Marketing Cloud Starter Data Bundles`?

- [x] `MobilePush`.
- [ ] `Personalization`.
- [x] `MobileConnect`.
- [ ] `Loyalty Management`.

### Northern Trail Outfitters unifies individuals in its `Data Cloud` instance. Which three features can the consultant use to validate the data on a unified profile?

- [ ] `Query API`.
- [x] `Data Explorer`.
- [x] `Identity Resolution`.
- [ ] `Data Actions`.
- [x] `Profile Explorer`.

### A consultant is integrating an Amazon S3 activated campaign with the customer's destination system. In order for the destination system to find the metadata about the segment, which file on the S3 will contain this information for processing?

- [x] The `.json` file.
- [ ] The `.txt` file.
- [ ] The `.zip` file.
- [ ] The `.csv` file.

### Which information is provided in a `.csv` file when activating to Amazon S3?

- [x] The activated data payload.
- [ ] An audit log showing the user who activated the segment and when it was activated.
- [ ] The manifest of origin sources within `Data Cloud`.
- [ ] The metadata regarding the segment definition.

### Which two common use cases can be addressed with `Data Cloud`?

- [ ] Safeguard critical business data by serving as a centralized system for backup and disaster recovery.
- [x] Harmonize data from multiple sources with a standardized and extendable data model.
- [x] Understand and act upon customer data to drive more relevant experiences.
- [ ] Govern enterprise data lifecycle through a centralized set of policies and processes.

### Northern Trail Outfitters (NTO) creates a calculated insight to compute recency, frequency, monetary (RFM) scores on its unified individuals. NTO then creates a segment based on these scores that it activates to a Marketing Cloud activation target. Which two actions are required when configuring the activation?

- [x] Select contact points.
- [ ] Add additional attributes.
- [x] Choose a segment.
- [ ] Add the calculated insight in the activation.

### Which data model subject area should be used for any Organization, Individual, or Member in the Customer 360 data model?

- [x] `Party`.
- [ ] `Global Account`.
- [ ] `Membership`.
- [ ] `Engagement`.

### The Salesforce CRM Connector is configured and the `Case` object data stream is set up. Subsequently, a new custom field named `Business Priority` is created on the `Case` object in Salesforce CRM. However, the new field is not available when trying to add it to the data stream. Which statement addresses the cause of this issue?

- [ ] The `Salesforce Data Loader` application should be used to perform a bulk upload from a desktop.
- [ ] After 24 hours when the data stream refreshes, it will automatically include any new fields that were added to the Salesforce CRM.
- [x] The `Salesforce Integration User` is missing `Read` permissions on the newly created field.
- [ ] Custom fields on the `Case` object are not supported for ingesting into `Data Cloud`.

### The marketing manager at Cloud Kicks plans to bring in corporate phone numbers for its accounts into `Data Cloud`. They plan to use a custom field with data set to Phone to store these phone numbers. Which statement is true when ingesting phone numbers?

- [x] Text value can be accepted for ingestion into = phone data type field.
- [ ] `Data Cloud` validates the format of the phone number at the time of Ingestion.
- [ ] The phone number field car only accept 10-digit values.
- [ ] The phone number field should be used as a primary key.

### What is a typical use case for `Salesforce Data Cloud`?

- [ ] Data synchronization across the Salesforce ecosystem.
- [ ] Storing CRM data on promises.
- [x] Data harmonization across multiple platforms.
- [ ] Sending personalized emails at scale.

### A consultant needs to create a data graph based on several DLOs, Which step should the consultant take to make this work?

- [ ] Use a data action to update the data graph with the DLO data.
- [x] Map the DLOS to DMOS and use these in the data graph.
- [ ] Map the DLOs directly to a data graph.
- [ ] Batch transform the DLOs to multiple DMOs and activate these with the data graph.

### Northern Trail Outfitters wants to create a segment with customers that have purchased in the last 24 hours. The segment data must be as up to date as possible. What should the consultant Implement when creating the segment?

- [x] Use streaming insights for near real-time segmentation results.
- [ ] Use Einstein segmentation optimization to collect data from the last 24 hours.
- [ ] Use rapid segments with a publish interval of 1 hour.
- [ ] Use standard segment with a publish interval of 30 minutes.

### An analyst from Cloud Kicks needs to get quick Insights to determine the average sales per day during the past week.What should a consultant recommend?

- [ ] Salesforce flows.
- [ ] Lightning web component utilizing `Query API`.
- [x] Salesforce reports.
- [ ] Segment activation to Azure.

### During an implementation project, a consultant completed ingestion of all data streams for their customer. Prior to segmenting and acting on that data, which additional configuration is required?

- [ ] `Data Activation`.
- [ ] `Calculated Insights`.
- [ ] `Data Mapping`.
- [x] `Identity Resolution`.

### Northern Trail Qutfitters wants to be able to calculate each customer's lifetime value (LTV) but also create breakdowns of the revenue sourced by website, mobile app, and retail channels. What should a consultant use to address this use case in `Data Cloud`?

- [ ] Flow Orchestration.
- [ ] Nested segments.
- [x] Metrics on metrics.
- [ ] Streaming data transform.

### A consultant wants to ensure that every segment managed by multiple brand teams adheres to the same set of axclusion criteria, that are updated on a monthly basis. What is the most efficient option to allow for this capability?

- [ ] Create, publish, and deploy a data kit.
- [x] Create a reusable container block with common criteria.
- [ ] Create a nested segment.
- [ ] Create a segment and copy it for each brand.

### A customer needs to integrate in real time with Salesforce CRM. Which feature accomplishes this requirement?

- [ ] Streaming transforms.
- [ ] Data model triggers.
- [ ] Sales and Service bundle.
- [ ] `Data Actions` and Lightning web components.

### A user wants to be able to create a multi-dimensional metric to identify `Unified Individual` lifetime value (LTV). Which sequence of Data Model Object (DMO) joins is necessary within the calculated Insight to enable this calculation?

- [x] `Unified Individual` > `Unified Link Individual` > `Sales Order`.
- [ ] `Unified Individual` > `Individual` > `Sales Order`.
- [ ] `Sales Order` > `Individual` > `Unified Individual`.
- [ ] `Sales Order` > `Unified Individual`.

### Cumulus Financial created a segment called `Multiple Investments` that contains individuals who have invested in two or more mutual funds. The company plans to send an email to this segment regarding a new mutual fund offering, and wants to personalize the email content with information about each customer's current mutual fund investments. How should the `Data Cloud` consultant configure this activation?

- [ ] Include `Fund Type` equal to `Mutual Fund` as a related attribute. Configure an activation based on the new segment with no additional attributes.
- [x] Choose the `Multiple Investments` segment, choose the `Email` contact point, add related attribute `Fund Name`, and add related attribute filter for `Fund Type` equal to `Mutual Fund`.
- [ ] Choose the `Multiple Investments` segment, choose the `Email` contact point, and add related attribute `Fund Type`.
- [ ] Include `Fund Name` and `Fund Type` by default for post processing in the target system.

### A segment fails to refresh with the error `Segment references too many data lake objects (DLOs)`. Which two troubleshooting tips should help remedy this issue?

- [ ] Split the segment into smaller segments.
- [ ] Use calculated insights in order to reduce the complexity of the segmentation query.
- [x] Refine segmentation criteria to limit up to five custom Data Model Objects (DMOs).
- [x] Space out the segment schedules to reduce DLO load.

### An organization wants to enable users with the ability to identify and select text attributes from a picklist of options. Which `Data Cloud` feature should help with this use case?

- [x] Value suggestion.
- [ ] Data harmonization.
- [ ] Transformation formulas.
- [ ] Global picklists.

### A consultant is working in a customer's `Data Cloud` org and is asked to delete the existing `Identity Resolution` ruleset. Which two impacts should the consultant communicate as a result of this action?

- [x] Unified customer data associated with this ruleset will be removed.
- [x] Dependencies on Data Model Objects will be removed.
- [ ] All individual data will be removed.
- [ ] All source profile data will be removed.

### Northern Trail Outfitters uploads new customer data to an Amazon S3 Bucket on a daily basis to be ingested in `Data Cloud`. In what order should each process be run to ensure that freshly imported data is ready and available to use for any segment?

- [ ] `Calculated Insight` > `Refresh Data Stream` > `Identity Resolution`.
- [ ] `Refresh Data Stream` > `Calculated Insight` > `Identity Resolution`.
- [ ] `Identity Resolution` > `Refresh Data Stream` > `Calculated Insight`.
- [x] `Refresh Data Stream` > `Identity Resolution` > `Calculated Insight`.

### Which two requirements must be met for a calculated insight to appear in the segmentation canvas?

- [x] The calculated insight must contain a dimension including the `Individual` or `Unified Individual ID`.
- [x] The primary key of the segmented table must be a dimension in the calculated insight.
- [ ] The metrics of the calculated insights must only contain numeric values.
- [ ] The primary key of the segmented table must be a metric in the calculated insight.

### A customer requests that their personal data be deleted. Which action should the consultant take to accommodate this request in `Data Cloud`?

- [ ] Use `Streaming API` call to delete the customer's information.
- [ ] Use `Profile Explorer` to delete the customer data from `Data Cloud`.
- [ ] Use `Consent API` to request deletion of the customer's information.
- [x] Use the `Data Rights Subject Request` tool to request deletion of the customer's information.

### What does the Ignore Empty Value option do in `Identity Resolution`?

- [ ] Ignores empty fields when running any custom match rules.
- [x] Ignores empty fields when running reconciliation rules.
- [ ] Ignores `Individual` object records with empty fields when running `Identity Resolution` rules.
- [ ] Ignores empty fields when running the standard match rules.

### Northern Trail Outfitters (NTO) is configuring an `Identity Resolution` ruleset based on `Fuzzy Name` and `Normalized Email`. What should NTO do to ensure the best email address is activated?

- [ ] Include `Contact Point Email` object `Is Active` field as a match rule.
- [x] Use the source priority order in activations to make sure a contact point from the desired source is delivered to the activation target.
- [ ] Ensure `Marketing Cloud` is prioritized as the first data source in the Source Priority reconciliation rule.
- [ ] Set the default reconciliation rule to `Last Updated`.

### A customer wants to create segments of users based on their `Customer Lifetime Value`. However, the source data that will be brought into `Data Cloud` does not include that key performance indicator (KPI). Which sequence of steps should the consultant follow to achieve this requirement?

- [x] `Ingest Data` > `Map Data to Data Model` > `Create Calculated Insight` > `Use in Segmentation`.
- [ ] `Create Calculated Insight` > `Map Data to Data Model` > `Ingest Data` > `Use in Segmentation`.
- [ ] `Create Calculated Insight` > `Ingest Data` > `Map Data to Data Model` > `Use in Segmentation`.
- [ ] `Ingest Data` > `Create Calculated Insight` > `Map Data to Data Model` > `Use in Segmentation`.

### During discovery, which feature should a consultant highlight for a customer who has multiple data sources and needs to match and reconcile data about individuals into a single unified profile?

- [x] Data Cleaning.
- [ ] Harmonization.
- [ ] Data Consolidation.
- [ ] `Identity Resolution`.

### Northern Trail Outfitters (NTO) wants to send a promotional campaign for customers that have purchased within the past 6 months. The consultant created a segment to meet this requirement. Now, NTO brings an additional requirement to suppress customers who have made purchases within the last week. What should the consultant use to remove the recent customers?

- [ ] Batch transforms.
- [x] Segmentation exclude rules.
- [ ] Related attributes.
- [ ] Streaming insight.

### Which data stream category should be assigned to use the data for time-based operations is segmentation and calculated insights?

- [ ] `Individual`.
- [ ] `Transaction`.
- [x] `Sales Order`.
- [ ] `Engagement`.

### Which method should a consultant use when performing aggregations in windows of 15 minutes on data collected via the Interaction SDK or Mobile SDK?

- [ ] Batch transform.
- [ ] Calculated insight.
- [x] Streaming insight.
- [ ] Formula fields.

### A customer has a custom `Customer Email c` object related to the standard `Contact` object in Salesforce CRM. This custom object stores the email address a Contact that they want to use for activation. To which data entity is mapped?

- [ ] `Contact`.
- [x] `Contact Point_Email`.
- [ ] `Custom customer Email__c` object.
- [ ] `Individual`.

### Every day, Northern Trail Outfitters uploads a summary of the last 24 hours of store transactions to a new file in an Amazon S3 bucket, and files older than seven days are automatically deleted. Each file contains a timestamp in a standardizel naming convention. Which two options should a consultant configure when ingesting this data stream?

- [ ] Ensure that deletion of old files is enabled.
- [x] Ensure the refresh mode is set to `Upsert`.
- [x] Ensure the filename contains a wildcard to a accommodate the timestamp.
- [ ] Ensure the refresh mode is set to `Full Refresh`.

### Which solution provides an easy way to ingest `Marketing Cloud` subscriber profile attributes into `Data Cloud` on a daily basis?

- [ ] `Automation Studio` and `Profile file API`.
- [ ] `Marketing Cloud Connect API`.
- [x] `Marketing Cloud Data` extension `Data Stream`.
- [ ] `Email Studio Started Data Bundle`.

### A customer has a requirement to be able to view the last time each segment was published within their `Data Cloud` org. Which two features should the consultant recommend to best address this requirement?

- [ ] `Profile Explorer`.
- [ ] `Calculated Insights`.
- [x] `Dashboard`.
- [x] `Report`.

### A `Data Cloud` consultant recently added a new data source and mapped some of the data to a new custom Data Model Object (DMO) that they want to use for creating segments. However, they cannot view the newly created DMO when trying to create a new segment. What is the cause of this issue?

- [ ] Data has not yet been ingested into the DMO.
- [x] The new DMO is not of category Profile.
- [ ] The new DMO does not have a relationship to the individual DMO.
- [ ] Segmentation is only supported for the Individual and `Unified Individual` DMOs.

### How does `Data Cloud` handle an individual's `Right to be Forgotten`?

- [ ] Deletes the record from all data source objects, and any downstream Data Model Objects are updated at the next schedulet ingestion.
- [ ] Deletes the specified Individual record and its `Unified Individual Link` record.
- [ ] Deletes the specified Individual and records from any data source object mapped to the Individual Data Model Object.
- [x] Deletes the specified Individual and records from any Data Model Object/data lake object related to the Individual.

### A healthcare client wants to make use of `Identity Resolution`, but does not want to risk unifying profiles that may share certain Personally Identifiable Information (PII). Which matching rule criteria should a consultant recommend for the most accurate matching results?

- [x] `Party Identification` on `Patient ID`.
- [ ] `Exact Last Name` and `Email`.
- [ ] `Email Address` and `Phone`.
- [ ] `Fuzzy First Name`, `Exact Last Name`, and `Email`.

### A user is not seeing suggested values from newly-modeled data when building a segment. What is causing this issue?

- [x] Value suggestion is still processing and to be available.
- [ ] Value suggestion requires `Data Aware Specialist` permissions at a minimum.
- [ ] Value suggestion can only work on direct attributes and not related attributes.
- [ ] Value suggestion will only return result for the first 50 values of a specific attribute.

### A consultant is building a segment to announce a new product launch for customers that have previously purchased black pants. How should the consultant place attributes for product color and product type from the `Order Product` object to meet this criteria?

- [ ] Place the attribute for product color in one container and the attribute for product type in another container.
- [ ] Place an attribute for the `black` calculated insight to dynamically apply.
- [ ] Place the attributes for product color and product type in a single container.
- [x] Place the attributes for product color and product type in a single container.

### Cumulus Financial wants to be able to track the daily transaction volume of each of its customers in real time and send out a notification as soon as it detects volume outside a customer's normal range. What should a consultant do to accommodate this request?

- [ ] Use a calculated insight paired with a flow.
- [ ] use streaming data transform with a flow.
- [x] Use a streaming insight paired with a data action.
- [ ] Use streaming data transform combined with a data action.

### Cumulus Financial uses calculated insights to compute the total banking value per branh for its high net worth customers. In the calculated insight, `banking value` is a metric, `branch` is a dimension, and `high net worth` is a filter. What can be included as an attribute in activation?

- [ ] `high net worth` (filter).
- [ ] `branch` (dimension) and (banking metric).
- [x] `banking value` (metric).
- [ ] `branch` (dimension).

### Cloud Kicks wants to be able to build a segment of customers who have visited its website within the previous 7 days. Which filter operator on the `Engagement Date` fields fits this use case?

- [ ] `Is Between`.
- [ ] `Greater than Last Number of`.
- [ ] `Next Number of Days`.
- [x] `Last Number of Days.`

### A `Data Cloud` consultant recently discovered that their `Identity Resolution` process is matching individual that share email addresses or phone numbers, but are not actually the same individual. What should the consultant do to address this issue?

- [ ] Modify the existing ruleset with stricter matching criteria, run the ruleset and review the updated results,then adjust as needed until the individuals are matching correctly.
- [x] Create and run a new rules fewer matching rules, compare the two rulesets to review and verify the results, and then migrate to the new ruleset once approved.
- [ ] Create and run a new ruleset with stricter matching criteria, compare the two rulesets to review and verify the results, and then migrate to the new ruleset once approved.
- [ ] Modify the existing ruleset with stricter matching criteria, compare the two rulesets to review  and verify the results, and then migrate to the new ruleset once approved.

### A retail customer wants to bring customer data from different sources and wants to take advantage of `Identity Resolution` so that it can be used in segmentation. On which entity should this be segmented for activation membership?

- [ ] `Subscriber`.
- [x] `Unified Individual`.
- [ ] `Unified Contact`.
- [ ] `Individual`.

### A consultant is reviewing a recent activation using engagement-based related attributes but is not seeing any related attributes in their payload for the majority of their segment members. Which two areas should the consultant review to help troubleshoot this issue?

- [x] The related engagement events occurred within the last 90 days.
- [ ] The activations are referencing segments that segment on profile data rather than engagement data.
- [x] The correct path is selected for the related attributes.
- [ ] The activated profiles have a `Unified Contact Point`.
