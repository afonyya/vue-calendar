<script lang="ts">
  import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'Calendar',
  });
</script>

<template>
  <div
    id="myDatepicker"
    class="datepicker"
  >
    <div class="date">
      <label for="id-textbox-1">Date</label>

      <div class="group">
        <input
          type="text"
          placeholder="mm/dd/yyyy"
          id="id-textbox-1"
          aria-describedby="id-description-1"
        />
        <span
          class="desc"
          id="id-description-1"
          >(<span class="sr-only">date format: </span>mm/dd/yyyy)</span
        >
        <button
          type="button"
          class="icon"
          aria-label="Choose Date"
        >
          <span class="fa fa-calendar-alt fa-2x"></span>
        </button>
      </div>
    </div>

    <div
      id="id-datepicker-1"
      class="datepicker-dialog"
      role="dialog"
      aria-modal="true"
      aria-label="Choose Date"
    >
      <div class="header">
        <button
          type="button"
          class="prev-year"
          aria-label="previous year"
        >
          <span class="fas fa-angle-double-left fa-lg"></span>
        </button>

        <button
          type="button"
          class="prev-month"
          aria-label="previous month"
        >
          <span class="fas fa-angle-left fa-lg"></span>
        </button>

        <h2
          id="id-grid-label"
          class="month-year"
          aria-live="polite"
        >
          February 2020
        </h2>

        <button
          type="button"
          class="next-month"
          aria-label="next month"
        >
          <span class="fas fa-angle-right fa-lg"></span>
        </button>

        <button
          type="button"
          class="next-year"
          aria-label="next year"
        >
          <span class="fas fa-angle-double-right fa-lg"></span>
        </button>
      </div>

      <div class="table-wrap">
        <table
          class="dates"
          role="grid"
          aria-labelledby="id-grid-label"
        >
          <thead>
            <tr>
              <th
                scope="col"
                abbr="Sunday"
              >
                Su
              </th>
              <th
                scope="col"
                abbr="Monday"
              >
                Mo
              </th>
              <th
                scope="col"
                abbr="Tuesday"
              >
                Tu
              </th>
              <th
                scope="col"
                abbr="Wednesday"
              >
                We
              </th>
              <th
                scope="col"
                abbr="Thursday"
              >
                Th
              </th>
              <th
                scope="col"
                abbr="Friday"
              >
                Fr
              </th>
              <th
                scope="col"
                abbr="Saturday"
              >
                Sa
              </th>
            </tr>
          </thead>

          <tbody>
            <tr>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                tabindex="-1"
                data-date="2020-02-01"
              >
                1
              </td>
            </tr>
            <tr>
              <td
                tabindex="-1"
                data-date="2020-02-02"
              >
                2
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-03"
              >
                3
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-04"
              >
                4
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-05"
              >
                5
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-06"
              >
                6
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-07"
              >
                7
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-08"
              >
                8
              </td>
            </tr>
            <tr>
              <td
                tabindex="-1"
                data-date="2020-02-09"
              >
                9
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-10"
              >
                10
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-11"
              >
                11
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-12"
              >
                12
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-13"
              >
                13
              </td>
              <td
                tabindex="0"
                data-date="2020-02-14"
                role="gridcell"
                aria-selected="true"
              >
                14
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-15"
              >
                15
              </td>
            </tr>
            <tr>
              <td
                tabindex="-1"
                data-date="2020-02-16"
              >
                16
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-17"
              >
                17
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-18"
              >
                18
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-19"
              >
                19
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-20"
              >
                20
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-21"
              >
                21
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-22"
              >
                22
              </td>
            </tr>
            <tr>
              <td
                tabindex="-1"
                data-date="2020-02-23"
              >
                23
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-24"
              >
                24
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-25"
              >
                25
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-26"
              >
                26
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-27"
              >
                27
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-28"
              >
                28
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-29"
              >
                29
              </td>
            </tr>
            <tr>
              <td
                tabindex="-1"
                data-date="2020-02-30"
              >
                30
              </td>
              <td
                tabindex="-1"
                data-date="2020-02-31"
              >
                31
              </td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
              <td
                class="disabled"
                tabindex="-1"
              ></td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="dialog-ok-cancel-group">
        <button
          class="dialog-button"
          value="cancel"
        >
          Cancel
        </button>
        <button
          class="dialog-button"
          value="ok"
        >
          OK
        </button>
      </div>
      <div
        class="dialog-message"
        aria-live="polite"
      ></div>
    </div>
  </div>
</template>

<style>
  .sr-only {
    position: absolute;
    top: -2000em;
    left: -3000em;
  }

  .datepicker {
    margin-top: 1em;
    position: relative;
  }

  .datepicker .group {
    display: inline-block;
    position: relative;
    width: 13em;
  }

  .datepicker label {
    display: block;
  }

  .datepicker input {
    padding: 0;
    margin: 0;
    height: 1.5em;
    background-color: white;
    color: black;
    border: 1px solid gray;
  }

  .datepicker button.icon {
    position: relative;
    top: 0.25em;
    margin: 0;
    padding: 4px;
    border: 0 solid #005a9c;
    background-color: white;
    border-radius: 5px;
  }

  .datepicker .desc {
    position: absolute;
    left: 0;
    top: 2em;
  }

  .datepicker .fa-calendar-alt {
    color: hsl(216deg 89% 51%);
  }

  .datepicker button.icon:focus {
    outline: none;
    padding: 2px;
    border-width: 2px;
    background-color: #def;
  }

  .datepicker input:focus {
    background-color: #def;
    outline: 2px solid #005a9c;
    outline-offset: 1px;
  }

  .datepicker-dialog {
    position: absolute;
    width: 320px;
    clear: both;
    border: 3px solid hsl(216deg 80% 51%);
    margin-top: 0.15em;
    border-radius: 5px;
    padding: 0;
    background-color: #fff;
  }

  .datepicker-dialog .header {
    cursor: default;
    background-color: hsl(216deg 80% 51%);
    padding: 7px;
    font-weight: bold;
    text-transform: uppercase;
    color: white;
    display: flex;
    justify-content: space-around;
  }

  .datepicker-dialog h2 {
    margin: 0;
    padding: 0;
    display: inline-block;
    font-size: 1em;
    color: white;
    text-transform: none;
    font-weight: bold;
    border: none;
  }

  .datepicker-dialog button {
    border-style: none;
    background: transparent;
  }

  .datepicker-dialog button::-moz-focus-inner {
    border: 0;
  }

  .datepicker-dialog .dates {
    width: 320px;
  }

  .datepicker-dialog .prev-year,
  .datepicker-dialog .prev-month,
  .datepicker-dialog .next-month,
  .datepicker-dialog .next-year {
    padding: 4px;
    width: 24px;
    height: 24px;
    color: white;
  }

  .datepicker-dialog .prev-year:focus,
  .datepicker-dialog .prev-month:focus,
  .datepicker-dialog .next-month:focus,
  .datepicker-dialog .next-year:focus {
    padding: 2px;
    border: 2px solid white;
    border-radius: 4px;
    outline: 0;
  }

  .datepicker-dialog .prev-year:hover,
  .datepicker-dialog .prev-month:hover,
  .datepicker-dialog .next-month:hover,
  .datepicker-dialog .next-year:hover {
    padding: 3px;
    border: 1px solid white;
    border-radius: 4px;
  }

  .datepicker-dialog .dialog-ok-cancel-group {
    text-align: right;
    margin-top: 1em;
    margin-bottom: 1em;
    margin-right: 1em;
  }

  .datepicker-dialog .dialog-ok-cancel-group button {
    padding: 6px;
    margin-left: 1em;
    width: 5em;
    background-color: hsl(216deg 80% 92%);
    font-size: 0.85em;
    color: black;
    outline: none;
    border-radius: 5px;
  }

  .datepicker-dialog .dialog-button:focus {
    padding: 4px;
    border: 2px solid black;
  }

  .datepicker-dialog .dialog-button:hover {
    padding: 5px;
    border: 1px solid black;
  }

  .datepicker-dialog .fa-calendar-alt {
    color: hsl(216deg 89% 51%);
  }

  .datepicker-dialog .month-year {
    display: inline-block;
    width: 12em;
    text-align: center;
  }

  .datepicker-dialog table.dates {
    padding-left: 1em;
    padding-right: 1em;
    padding-top: 1em;
    border: none;
    border-collapse: separate;
  }

  .datepicker-dialog table.dates th,
  .datepicker-dialog table.dates td {
    text-align: center;
    background: white;
    color: black;
    border: none;
  }

  .datepicker-dialog table.dates tr {
    border: 1px solid black;
  }

  .datepicker-dialog table.dates td {
    padding: 3px;
    margin: 0;
    line-height: inherit;
    height: 40px;
    width: 40px;
    border-radius: 5px;
    font-size: 15px;
    background: #eee;
  }

  .datepicker-dialog table.dates td.disabled {
    padding: 2px;
    border: none;
    height: 41px;
    width: 41px;
  }

  .datepicker-dialog table.dates td:focus,
  .datepicker-dialog table.dates td:hover {
    padding: 0;
    background-color: hsl(216deg 80% 92%);
    color: black;
  }

  .datepicker-dialog table.dates td:focus {
    padding: 1px;
    border: 2px solid rgb(100 100 100);
    outline: 0;
  }

  .datepicker-dialog table.dates td:not(.disabled):hover {
    padding: 2px;
    border: 1px solid rgb(100 100 100);
  }

  .datepicker-dialog table.dates td[aria-selected] {
    padding: 1px;
    border: 2px dotted rgb(100 100 100);
  }

  .datepicker-dialog table.dates td[aria-selected]:focus {
    padding: 1px;
    border: 2px solid rgb(100 100 100);
  }

  .datepicker-dialog table.dates td[tabindex='0'] {
    background-color: hsl(216deg 80% 51%);
    color: white;
  }

  .datepicker-dialog .dialog-message {
    padding-top: 0.25em;
    padding-left: 1em;
    height: 1.75em;
    background: hsl(216deg 80% 51%);
    color: white;
  }
</style>
