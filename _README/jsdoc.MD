# jsDoc

If planning to produce documentation, use jsDoc syntax to document function names, description, params and returns. Use @namespace and @memberOf to match your app structure.

Why?: You can generate (and regenerate) documentation from your code, instead of writing it from scratch.

Why?: Provides consistency using a common industry tool.

````{
/**
 * Logger Factory
 * @namespace Factories
 */
(function() {
  angular
      .module('app')
      .factory('logger', logger);

  /**
   * @namespace Logger
   * @desc Application wide logger
   * @memberOf Factories
   */
  function logger($log) {
      var service = {
         logError: logError
      };
      return service;

      ////////////

      /**
       * @name logError
       * @desc Logs errors
       * @param {String} msg Message to log
       * @returns {String}
       * @memberOf Factories.Logger
       */
      function logError(msg) {
          var loggedMsg = 'Error: ' + msg;
          $log.error(loggedMsg);
          return loggedMsg;
      };
  }
})();
}````