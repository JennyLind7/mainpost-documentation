## Absences

Absences reflect person-related absences such as sickness and holidays.

<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>DataType</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
   <tr>
      <td>number</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>employee_id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>allocation_id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>reason</td>
      <td>character varying</td>
      <td>Sick or on holiday</td>
    </tr>
    <tr>
      <td>start_date</td>
      <td>date</td>
      <td></td>
    </tr>
    <tr>
      <td>end_date</td>
      <td>date</td>
      <td></td>
    </tr>
    <tr>
      <td>temporary</td>
      <td>boolean</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Allocations

<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>DataType</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>employee_id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>round_id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>round_code</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>district_id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>start_date</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>end_date</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>level</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>training</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>day_delivery</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>deposition_zip</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>deposition_city</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>deposition_district</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>deposition_street</td>
      <td>text</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Rounds

<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>DataType</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>code</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>start_date</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>end_date</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>monday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>tuesday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>wednesday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>thursday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>friday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>saturday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>sunday</td>
      <td>boolean</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Districts
<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>DataType</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>bigint</td>
      <td>generated by default as identity</td>
    </tr>
    <tr>
      <td>name</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>alias</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>round</td>
      <td>text</td>
      <td>Current round combination</td>
    </tr>
    <tr>
      <td>realm</td>
      <td>text</td>
      <td>Town and district (if available)</td>
    </tr>
    <tr>
      <td>active_since</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>split_allowed</td>
      <td>boolean</td>
      <td>Defines whether it is allowed to deliver the district in different delivery accesses</td>
    </tr>
    <tr>
      <td>area_id</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>shelf</td>
      <td>text</td>
      <td>Wagon compartment number, where the letters are sorted or picked up</td>
    </tr>
    <tr>
      <td>is_old_district</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>avg_hours_old_districts</td>
      <td>double precision</td>
      <td></td>
    </tr>
    <tr>
      <td>avg_length_old_districts</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>vehicle_letter</td>
      <td>text</td>
      <td>Current transport vehicle</td>
    </tr>
    <tr>
      <td>vehicle_optimal_letter</td>
      <td>text</td>
      <td>Current or optimal transport vehicle</td>
    </tr>
    <tr>
      <td>vehicle_newspaper</td>
      <td>text</td>
      <td>Current transport vehicle</td>
    </tr>
    <tr>
      <td>vehicle_optimal_newspaper</td>
      <td>text</td>
      <td>Current or optimal transport vehicle</td>
    </tr>
    <tr>
      <td>newspapers</td>
      <td>text</td>
      <td>Ø Number of newspapers</td>
    </tr>
    <tr>
      <td>letters</td>
      <td>bigint</td>
      <td>Ø Number of letters</td>
    </tr>
    <tr>
      <td>direct</td>
      <td>text</td>
      <td>Ø Number of direct distributions (magazines)</td>
    </tr>
    <tr>
      <td>direct_per_year</td>
      <td>text</td>
      <td>Ø Days of direct distribution (magazines) per year</td>
    </tr>
    <tr>
      <td>meters_newspapers</td>
      <td>text</td>
      <td>Route for individual rounds within the district</td>
    </tr>
    <tr>
      <td>meters_letters</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>meters_dual</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>letter_district_surcharge</td>
      <td>text</td>
      <td>District-related surcharge if district is longer than actually planned and not yet remeasured</td>
    </tr>
    <tr>
      <td>newspaper_district_surcharge</td>
      <td>text</td>
      <td>District-related surcharge if district is longer than actually planned and not yet remeasured</td>
    </tr>
    <tr>
      <td>letter_employee_surcharge</td>
      <td>text</td>
      <td>Person-related surcharge (for current regular delivery staff) for handicap e.g.</td>
    </tr>
    <tr>
      <td>newspaper_employee_surcharge</td>
      <td>text</td>
      <td>Person-related surcharge (for current regular delivery staff) for handicap e.g.</td>
    </tr>
  </tbody>
</table>

## Employee
<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>DataType</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>weekly_hours</td>
      <td>text</td>
      <td>Only set for full-time/part-time employees</td>
    </tr>
    <tr>
      <td>type</td>
      <td>text</td>
      <td>'default', 'auxiliary', 'time-based', 'variable'</td>
    </tr>
    <tr>
      <td>freelancer</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>monday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>tuesday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>wednesday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>thursday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>friday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>saturday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>sunday</td>
      <td>boolean</td>
      <td></td>
    </tr>
    <tr>
      <td>birthday</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>expiration</td>
      <td>text</td>
      <td>Exit date</td>
    </tr>
    <tr>
      <td>expiration_reason</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>nationality</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>date_of_joining</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>residence_zip</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>residence_city</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>residence_district</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>residence_street</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>residence_latitude</td>
      <td>text</td>
      <td></td>
    </tr>
    <tr>
      <td>residence_longitude</td>
      <td>text</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Vacancies
Vacancies reflect the round-specific absences such as work prohibition, not worn, etc.
<table>
  <thead>
    <tr>
      <th>Feature</th>
      <th>DataType</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>bigint</td>
      <td></td>
    </tr>
    <tr>
      <td>allocation_id</td>
      <td>bigint</td>
      <td>There is always an allocation for failure</td>
    </tr>
    <tr>
      <td>reason</td>
      <td>text</td>
      <td>Reason for failure: Not delivered, work ban, other</td>
    </tr>
    <tr>
      <td>start_date</td>
      <td>date</td>
      <td></td>
    </tr>
    <tr>
      <td>end_date</td>
      <td>date</td>
      <td></td>
    </tr>
  </tbody>
</table>













