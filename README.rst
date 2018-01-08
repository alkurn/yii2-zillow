Zillow, PHP Wrapper
================================

This is a simple PHP Wrapper for the Zillow API services.

.. image:: https://travis-ci.org/alkurn/zillow.svg?branch=master
    :target: https://travis-ci.org/alkurn/zillow

Requirements
------------

depends on PHP 5.4+, Goutte 2.0+, Guzzle 4+.

Installation
------------

Add `alkurn/yii2-zillow` as a require dependency in your ``composer.json`` file:

.. code-block:: bash

    composer require alkurn/yii2-zillow:dev-master

Usage
-----

.. code-block:: php

    use Zillow\ZillowClient;

    $client = new ZillowClient('ZWSID');

Make requests with a specific API call method:

.. code-block:: php

    // Run GetSearchResults
    $response = $client->GetSearchResults(['address' => '5400 Tujunga Ave', 'citystatezip' => 'North Hollywood, CA 91601']);

Any Zillow API call will work. Valid callbacks are:

- GetZestimate
- GetSearchResults
- GetChart
- GetComps
- GetDeepComps
- GetDeepSearchResults
- GetUpdatedPropertyDetails
- GetDemographics
- GetRegionChildren
- GetRegionChart
- GetRateSummary
- GetMonthlyPayments
- CalculateMonthlyPaymentsAdvanced
- CalculateAffordability
- CalculateRefinance
- CalculateAdjustableMortgage
- CalculateMortgageTerms
- CalculateDiscountPoints
- CalculateBiWeeklyPayment
- CalculateNoCostVsTraditional
- CalculateTaxSavings
- CalculateFixedVsAdjustableRate
- CalculateInterstOnlyVsTraditional
- CalculateHELOC


License
-------

MIT license.
