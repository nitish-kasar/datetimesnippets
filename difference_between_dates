<?php 

/* Get Difference between two dates in days  */

$end_date = new DateTime([DATE_ONE_HERE]);    
$current_date = new DateTime([DATE_TWO_HERE]);

$interval = $current_date->diff($end_date);

$days = (int)$interval->days;

/* Adjustment for date just after current date */
if($interval->invert==0 && $interval->days==0)
{
    $days+=1;
}    

/* Adjustment for representing negative date difference */
elseif ($interval->invert==1) 
{
    $days = -(int)$interval->days;
} 
