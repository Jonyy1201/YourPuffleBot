package nu.glen.yourpufflebot 

import nu.glen.followbackbot.{
  BeHaveDoKeywordPrefixResponder,
  GerrundKeywordPrefixResponder,
  PastTenseKeywordPrefixResponder
}

class YourPuffleGerrundResponder extends GerrundKeywordPrefixResponder {
  override def combine(gerrund: String, rest: String) = "Your puffle's %s%s".format(gerrund, rest)
}

class YourPufflePastTenseResponder extends PastTenseKeywordPrefixResponder {
  override def combine(verb: String, rest: String) = "Your puffle %s%s".format(verb, rest)
}

class YourPuffleBeHaveDoResponder extends BeHaveDoKeywordPrefixResponder {
  override def combine(verb: String, rest: String) = "Your puffle %s%s".format(verb, rest)
