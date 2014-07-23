![ATIONET](Content/Images/ATIOnetLogo_250x70.png) 

***

#ATIOnet Fleet Organization

> **About:** This document explains the different criteria and tools to map a complex or large fleet of vehicles to ATIOnet, to simplify its administration and control.   	

</br>

<table>
	<thead>
		<tr>
			<td colspan="2" class="tablehead">Document Information</td>
		</tr>
	</thead>
	<tfoot>
		<td colspan="2"> </td>
	</tfoot>
	<tbody>
		<tr>
			<td width="20%" class="rowhead" align="right">File:</td>
			<td>AN-Fleet_Organization-TechGuide.en.md</td>
		</tr>
		<tr>
			<td align="right">Doc. Version:</td>
			<td>1.0</td>
		</tr>
		<tr>
			<td align="right">Release Date:</td>
			<td>20/July/2014</td>
		</tr>
		<tr>
			<td align="right">Author:</td>
			<td>ATIO International LLC</td>
		</tr>
	</tbody>
</table>

<table>
     <thead>
          <tr>
          	<td colspan="3">Change Log</td>
          </tr>
     </thead>
     <tfoot>
          <td colspan="3"> </td>
     </tfoot>
     <tbody>
        <tr>
          	<td>Ver.</td>
            <td>Date</td>
            <td>Change summary</td>
        </tr>
        <!-- Insert a table row like this for each version -->
        <tr>
          	<td>1.0</td>
          	<td>20/July/2014</td>
          	<td>Initial version</td>
        </tr>
        <!-- End of version table row -->
     </tbody>
</table>
</br>

<!--###Table of Content -->


<!-- Optional Terms & Definition section -->
        

<!-- Content starts here -->
##Units##
ATIOnet recognizes two types of _cardholders_: Persons and Units, usually called Drivers and Vehicles in the retail petroleum industry. Both _persons_ and _units_ can be the subject of a transaction and are considered a _sub-account_, within a contract with a Company.
Besides the obvious particularities between the configuration attributes of a Person and a Unit, a major difference is that Units can be organized in **Fleets**.   
Units can be trucks, cars, ships, planes, stationary machinery, generators or any other kind of device that may be identified as the beneficiary (subject) of an ATIOnet transaction.

###Classification and grouping attributes###

| Attribute                                  | Description                                                          |
| ------------------------------------------ | -------------------------------------------------------------------- |
| Code                                       | Main identification key of the Unit, alphanumeric value must be unique on the Company. Should be reserved for the actual number or code for the unit on the organization. When used on filters and searches, entering a part of the code would work as a wildcard (for example entering "RT" will work as RT*, returning all units with Code starting with "RT") |
| Fleet                                      | Highest level grouping entity. A Unit must belong to a Fleet and to one fleet only.|
| Vehicle Class                              | Every Unit belogs to a Vehicle Class. The Class resumes some attributes related to the Unit brand/model, like fuel type or fuel capacity|
| Type (in Vehicle Class)                    | The Type of Unit is a broad classification (Light Truck, Heavy Truck, Car, etc.) |
| Classification 1 to 4                      | Each Company can define up to 4 named classification attributes according to their own needs and policies. Can be used to describe operational regions, sub-type of units, type of service, cost centers, budgetary class, etc.|
| Service Type                               | Tipified description of the service to which this Unit is assigned. The Service Type, combined with the Vehicle Class will enable anonymous mileage benchmarking with other ATIOnet subscribers|
| Service Description                        | Label. Free description of the assigned service (route, schedule, etc.)|

##Fleet administration##
Once the list of Units is loaded ready on ATIOnet, the Fleet maintenance requirements can be classified in:

2. Managing balances
3. Managing Identifications
4. Managing restrictions and rules
5. Reporting

Balances need attention only when the Contract is set to _Balance Dispersion Mode_. In this case, a Company Admin have to take care of transferring funds -or product volume- from the Contract to the Unit's sub-account. When the Contract is set to _Do not disperse Mode_, ATIOnet automatically withdraws transaction funds from the Contract's main account, and the regular flow of payments from the Fleet Company to the Subscriber is enough to maintain the balances in order.

Identifications are the cards, TAGs, keys or any other device, media support or piece of information that can be used to identify a card-holder, in this case a Unit. Usually, Identifications are assigned to the Units when they begin to use the system, but from time to time, Identifications may require some administration, for example to disable a broken card, claim a stolen or lost ID, or to reasign it from one unit to other when the Identification is reusable. 
The union of a Unit with an Identification defines a _sub-account_ of a Contract. A given Unit might have more than one Identification, for example, because it have ring-TAGs and the unit have more than one fuel tank, or because the unit has a pre-paid disposable card as a contingency of the main account.
On any case, Identification is managed at the Unit -or Person- level, ATIOnet provides tools to ease the administration of Identifications but no grouping or classification applies to this relation.
A Company also might have more than one Contract with a Subscriber, this is useful to represent the departamental budgets on a corporate-wide agreement, or to split between Credit and Debit agreements with the same customer (fleet company), or another business terms. _Contracts are a business tool_

Reporting and Rules management are the areas where a good classification and planning pays-off.
Rules can be applied to Fleets, Custom Classification Fields (CCFs) and Units. All of them, plus the Service-type and Service-description can be used as filters for Units administration and reporting filters. And there is no one-fits-to-all recipe on how to use them.

![Fleet Administration Diagram](/Content/Includes/AN-Fleet_Organization-TechGuide-diagram.png)

##Fleet organization##

_Fleets are a hierarchical organization tool_. The Fleet Admin role can be delegated from the parent Company Admin role, and a Unit belongs only to one Fleet. Therefore, the Fleet should be mapped to the actual fleet operation structure, for example the, service base, logistic unit, etc. Fleet Admin users can re-configure the Units, assign rules, assign available Identifiers, assign Drivers, and the rest of the day-to-day functions. Except for widely distributed organizations, where a large number of fleets will be created, the Fleet level is too important to be used just for rules assignment.

_Vehicle classes could solve the basic fuel product and transaction limit_. Unless there is too much dispersion on the brands and models of the units, assigning a Vehicle Class during the creation of the unit will avoid to apply a Product Rule and a Transaction Limit Rule (at least as a security procedure). Vehicle classes are maintained by each fleet company, so each one can configure its own classes and not necessarily following an actual brand/model (for example, there are different brands of diesel pickups with same consumption, and fuel grade).

_Custom Classification Fields_ can be used as a filtering tool on reports and administrative views but also to apply Rules. Once a CCF is named by a Company Admin user, that label is used accross the system for all the users of the Company. CCF can be used to map the organization or budget structure, service type (route, zone, service hours), fleet sub-divisions or any other classification purpose. CCF are optionals from one to four and don't have a hierarchical structure.



 







