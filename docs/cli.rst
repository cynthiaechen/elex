======================
Command line interface
======================

------------------
Commands and flags
------------------

::

    commands:

      ballot-measures
        Get ballot measures

      candidate-reporting-units
        Get candidate reporting units (without results)

      candidates
        Get candidates

      clear-delegate-cache
        Clear the delegate report ID cache.

      delegates
        Get all delegate reports

      elections
        Get list of available elections

      next-election
        Get the next election (if date is specified, will be relative to that date, otherwise will use today's date)

      races
        Get races

      reporting-units
        Get reporting units

      results
        Get results

    positional arguments:
      date                  Election date (e.g. "2015-11-03"; most common date
                            formats accepted).

    optional arguments:
      -h, --help            show this help message and exit
      --debug               toggle debug output
      --quiet               suppress all output
      -o {csv,json}         output format (default: csv)
      -t, --test            Use testing API calls
      -n, --not-live        Do not use live data API calls
      -d DATA_FILE, --data-file DATA_FILE
                            Specify data file instead of making HTTP request when
                            using election commands like `elex results` and `elex
                            races`.
      --delegate-sum-file DELEGATE_SUM_FILE
                            Specify delegate sum report file instead of making
                            HTTP request when using `elex delegates`
      --delegate-super-file DELEGATE_SUPER_FILE
                            Specify delegate super report file instead of making
                            HTTP request when using `elex delegates`
      --format-json         Pretty print JSON when using `-o json`.
      -v, --version         show program's version number and exit
      --results-level RESULTS_LEVEL
                            Specify reporting level for results
      --set-zero-counts     Override results with zeros; omits the winner
                            indicator.Sets the vote, delegate, and reporting
                            precinct counts to zero.
      --local-only          Limit results to local-level results only.
      --with-timestamp      Append a `timestamp` column to each row of data output
                            with current system timestamp.
      --batch-name BATCH_NAME
                            Specify a value for a `batchname` column to append to
                            each row.


-----------------
Command reference
-----------------

.. autoclass:: elex.cli.app.ElexBaseController
    :members:
