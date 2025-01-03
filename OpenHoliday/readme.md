# PacketParser Templates for TapHome

Open Holidays API is used to determine whether the current day is a public holiday or a school holiday based on country and region.

## Module Variables
Module is predefined for Slovakia/Banska Bystrica region.
In order to make module to work correctly, module variables have to be modified according to the country and region.

<b>Country</b><br/>
Set the Country iso code based on the list from the URL: https://openholidaysapi.org/Countries<br/><br/>
<b>Region</b><br/>
Set the Region iso code based on list from this url: https://openholidaysapi.org/Subdivisions?countryIsoCode=<i>{CountryIsoCode}</i> <br/>
for Slovakia it is https://openholidaysapi.org/Subdivisions?countryIsoCode=SK

## Module Devices
<ul>
<li>IsPublicHoliday - boolean - the current day is a public holiday based on a country/region</li>
<li>IsSchoolHoliday - boolean - the current day is a school holiday based on a country/region</li>
<li>IsWeekend - boolean - the current day is a weekend day</li>
</ul>

