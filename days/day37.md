# Day 37

I hate Xcode... well, not entirely, but it does give me a headache. I got my form generated and just the way I like it, and after making a small tweek to a control, my solution would build, but no longer work. This sucks, because I worked late last night in getting the UI to just where I wanted it. 

This afternoon, I am going to take a break from Visusal Studio.Mac and XCode and instead start looking at the docker container I pulled down from Stanford. Perhaps just play around with the sentiment anaylis engine I have. After all, Docker Con starts bright and early in the morning tommorrow. 


Started playing... holy cow... still has some test cases and what not, but it was real easy to run....

'''json
Lukass-iMac:~ lukasliukonen$ curl --data 'I am glad that I got my Docker image working, and validating that it comes back with values!' 'http://192.168.11.28:9000/?properties={%22annotators%22%3A%22sentiment%22%2C%22outputFormat%22%3A%22json%22}' -o -
{
  "sentences": [
    {
      "index": 0,
      "parse": "(ROOT\n  (S\n    (S\n      (NP (PRP I))\n      (VP (VBP am)\n        (ADJP (JJ glad)\n          (SBAR (IN that)\n            (S\n              (NP (PRP I))\n              (VP (VBD got)\n                (NP (PRP$ my) (NNP Docker) (NN image) (NN working))))))))\n    (, ,)\n    (CC and)\n    (S\n      (VP (VBG validating)\n        (SBAR (IN that)\n          (S\n            (NP (PRP it))\n            (VP (VBZ comes)\n              (ADVP (RB back))\n              (PP (IN with)\n                (NP (NNS values))))))))\n    (. !)))",
      "basicDependencies": [
        {
          "dep": "ROOT",
          "governor": 0,
          "governorGloss": "ROOT",
          "dependent": 3,
          "dependentGloss": "glad"
        },
        {
          "dep": "nsubj",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 1,
          "dependentGloss": "I"
        },
        {
          "dep": "cop",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 2,
          "dependentGloss": "am"
        },
        {
          "dep": "mark",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 4,
          "dependentGloss": "that"
        },
        {
          "dep": "nsubj",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 5,
          "dependentGloss": "I"
        },
        {
          "dep": "ccomp",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 6,
          "dependentGloss": "got"
        },
        {
          "dep": "nmod:poss",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 7,
          "dependentGloss": "my"
        },
        {
          "dep": "compound",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 8,
          "dependentGloss": "Docker"
        },
        {
          "dep": "compound",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 9,
          "dependentGloss": "image"
        },
        {
          "dep": "dobj",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 10,
          "dependentGloss": "working"
        },
        {
          "dep": "punct",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 11,
          "dependentGloss": ","
        },
        {
          "dep": "cc",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 12,
          "dependentGloss": "and"
        },
        {
          "dep": "conj",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 13,
          "dependentGloss": "validating"
        },
        {
          "dep": "mark",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 14,
          "dependentGloss": "that"
        },
        {
          "dep": "nsubj",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 15,
          "dependentGloss": "it"
        },
        {
          "dep": "ccomp",
          "governor": 13,
          "governorGloss": "validating",
          "dependent": 16,
          "dependentGloss": "comes"
        },
        {
          "dep": "advmod",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 17,
          "dependentGloss": "back"
        },
        {
          "dep": "case",
          "governor": 19,
          "governorGloss": "values",
          "dependent": 18,
          "dependentGloss": "with"
        },
        {
          "dep": "nmod",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 19,
          "dependentGloss": "values"
        },
        {
          "dep": "punct",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 20,
          "dependentGloss": "!"
        }
      ],
      "enhancedDependencies": [
        {
          "dep": "ROOT",
          "governor": 0,
          "governorGloss": "ROOT",
          "dependent": 3,
          "dependentGloss": "glad"
        },
        {
          "dep": "nsubj",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 1,
          "dependentGloss": "I"
        },
        {
          "dep": "nsubj",
          "governor": 13,
          "governorGloss": "validating",
          "dependent": 1,
          "dependentGloss": "I"
        },
        {
          "dep": "cop",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 2,
          "dependentGloss": "am"
        },
        {
          "dep": "mark",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 4,
          "dependentGloss": "that"
        },
        {
          "dep": "nsubj",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 5,
          "dependentGloss": "I"
        },
        {
          "dep": "ccomp",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 6,
          "dependentGloss": "got"
        },
        {
          "dep": "nmod:poss",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 7,
          "dependentGloss": "my"
        },
        {
          "dep": "compound",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 8,
          "dependentGloss": "Docker"
        },
        {
          "dep": "compound",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 9,
          "dependentGloss": "image"
        },
        {
          "dep": "dobj",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 10,
          "dependentGloss": "working"
        },
        {
          "dep": "punct",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 11,
          "dependentGloss": ","
        },
        {
          "dep": "cc",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 12,
          "dependentGloss": "and"
        },
        {
          "dep": "conj:and",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 13,
          "dependentGloss": "validating"
        },
        {
          "dep": "mark",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 14,
          "dependentGloss": "that"
        },
        {
          "dep": "nsubj",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 15,
          "dependentGloss": "it"
        },
        {
          "dep": "ccomp",
          "governor": 13,
          "governorGloss": "validating",
          "dependent": 16,
          "dependentGloss": "comes"
        },
        {
          "dep": "advmod",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 17,
          "dependentGloss": "back"
        },
        {
          "dep": "case",
          "governor": 19,
          "governorGloss": "values",
          "dependent": 18,
          "dependentGloss": "with"
        },
        {
          "dep": "nmod:with",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 19,
          "dependentGloss": "values"
        },
        {
          "dep": "punct",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 20,
          "dependentGloss": "!"
        }
      ],
      "enhancedPlusPlusDependencies": [
        {
          "dep": "ROOT",
          "governor": 0,
          "governorGloss": "ROOT",
          "dependent": 3,
          "dependentGloss": "glad"
        },
        {
          "dep": "nsubj",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 1,
          "dependentGloss": "I"
        },
        {
          "dep": "nsubj",
          "governor": 13,
          "governorGloss": "validating",
          "dependent": 1,
          "dependentGloss": "I"
        },
        {
          "dep": "cop",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 2,
          "dependentGloss": "am"
        },
        {
          "dep": "mark",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 4,
          "dependentGloss": "that"
        },
        {
          "dep": "nsubj",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 5,
          "dependentGloss": "I"
        },
        {
          "dep": "ccomp",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 6,
          "dependentGloss": "got"
        },
        {
          "dep": "nmod:poss",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 7,
          "dependentGloss": "my"
        },
        {
          "dep": "compound",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 8,
          "dependentGloss": "Docker"
        },
        {
          "dep": "compound",
          "governor": 10,
          "governorGloss": "working",
          "dependent": 9,
          "dependentGloss": "image"
        },
        {
          "dep": "dobj",
          "governor": 6,
          "governorGloss": "got",
          "dependent": 10,
          "dependentGloss": "working"
        },
        {
          "dep": "punct",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 11,
          "dependentGloss": ","
        },
        {
          "dep": "cc",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 12,
          "dependentGloss": "and"
        },
        {
          "dep": "conj:and",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 13,
          "dependentGloss": "validating"
        },
        {
          "dep": "mark",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 14,
          "dependentGloss": "that"
        },
        {
          "dep": "nsubj",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 15,
          "dependentGloss": "it"
        },
        {
          "dep": "ccomp",
          "governor": 13,
          "governorGloss": "validating",
          "dependent": 16,
          "dependentGloss": "comes"
        },
        {
          "dep": "advmod",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 17,
          "dependentGloss": "back"
        },
        {
          "dep": "case",
          "governor": 19,
          "governorGloss": "values",
          "dependent": 18,
          "dependentGloss": "with"
        },
        {
          "dep": "nmod:with",
          "governor": 16,
          "governorGloss": "comes",
          "dependent": 19,
          "dependentGloss": "values"
        },
        {
          "dep": "punct",
          "governor": 3,
          "governorGloss": "glad",
          "dependent": 20,
          "dependentGloss": "!"
        }
      ],
      "sentimentValue": "3",
      "sentiment": "Positive",
      "sentimentDistribution": [
        0.00411293184642,
        0.00371670937913,
        0.00490059916883,
        0.52387283070467,
        0.46339692890095
      ],
      "sentimentTree": "(ROOT|sentiment=3|prob=0.524\n  (@S|sentiment=3|prob=0.614\n    (@S|sentiment=3|prob=0.664\n      (@S|sentiment=3|prob=0.490\n        (S|sentiment=3|prob=0.473 (NP|sentiment=2|prob=0.996 I)\n          (VP|sentiment=3|prob=0.510 (VBP|sentiment=2|prob=0.957 am)\n            (ADJP|sentiment=3|prob=0.615 (JJ|sentiment=2|prob=0.770 glad)\n              (SBAR|sentiment=3|prob=0.687 (IN|sentiment=2|prob=0.991 that)\n                (S|sentiment=3|prob=0.723 (NP|sentiment=2|prob=0.996 I)\n                  (VP|sentiment=3|prob=0.650 (VBD|sentiment=2|prob=0.995 got)\n                    (NP|sentiment=2|prob=0.855 (PRP$|sentiment=2|prob=0.998 my)\n                      (@NP|sentiment=2|prob=0.762 (NNP|sentiment=2|prob=0.631 Docker)\n                        (@NP|sentiment=2|prob=0.971 (NN|sentiment=2|prob=0.987 image) (NN|sentiment=2|prob=0.989 working))))))))))\n        (,|sentiment=2|prob=0.997 ,))\n      (CC|sentiment=2|prob=0.996 and))\n    (S|sentiment=3|prob=0.482 (VBG|sentiment=2|prob=0.631 validating)\n      (SBAR|sentiment=3|prob=0.591 (IN|sentiment=2|prob=0.991 that)\n        (S|sentiment=3|prob=0.614 (NP|sentiment=2|prob=0.993 it)\n          (VP|sentiment=3|prob=0.540\n            (@VP|sentiment=2|prob=0.716 (VBZ|sentiment=3|prob=0.958 comes) (ADVP|sentiment=2|prob=0.997 back))\n            (PP|sentiment=2|prob=0.792 (IN|sentiment=2|prob=0.992 with) (NP|sentiment=2|prob=0.993 values)))))))\n  (.|sentiment=2|prob=0.999 !))",
      "tokens": [
        {
          "index": 1,
          "word": "I",
          "originalText": "I",
          "characterOffsetBegin": 0,
          "characterOffsetEnd": 1,
          "pos": "PRP",
          "before": "",
          "after": " "
        },
        {
          "index": 2,
          "word": "am",
          "originalText": "am",
          "characterOffsetBegin": 2,
          "characterOffsetEnd": 4,
          "pos": "VBP",
          "before": " ",
          "after": " "
        },
        {
          "index": 3,
          "word": "glad",
          "originalText": "glad",
          "characterOffsetBegin": 5,
          "characterOffsetEnd": 9,
          "pos": "JJ",
          "before": " ",
          "after": " "
        },
        {
          "index": 4,
          "word": "that",
          "originalText": "that",
          "characterOffsetBegin": 10,
          "characterOffsetEnd": 14,
          "pos": "IN",
          "before": " ",
          "after": " "
        },
        {
          "index": 5,
          "word": "I",
          "originalText": "I",
          "characterOffsetBegin": 15,
          "characterOffsetEnd": 16,
          "pos": "PRP",
          "before": " ",
          "after": " "
        },
        {
          "index": 6,
          "word": "got",
          "originalText": "got",
          "characterOffsetBegin": 17,
          "characterOffsetEnd": 20,
          "pos": "VBD",
          "before": " ",
          "after": " "
        },
        {
          "index": 7,
          "word": "my",
          "originalText": "my",
          "characterOffsetBegin": 21,
          "characterOffsetEnd": 23,
          "pos": "PRP$",
          "before": " ",
          "after": " "
        },
        {
          "index": 8,
          "word": "Docker",
          "originalText": "Docker",
          "characterOffsetBegin": 24,
          "characterOffsetEnd": 30,
          "pos": "NNP",
          "before": " ",
          "after": " "
        },
        {
          "index": 9,
          "word": "image",
          "originalText": "image",
          "characterOffsetBegin": 31,
          "characterOffsetEnd": 36,
          "pos": "NN",
          "before": " ",
          "after": " "
        },
        {
          "index": 10,
          "word": "working",
          "originalText": "working",
          "characterOffsetBegin": 37,
          "characterOffsetEnd": 44,
          "pos": "NN",
          "before": " ",
          "after": ""
        },
        {
          "index": 11,
          "word": ",",
          "originalText": ",",
          "characterOffsetBegin": 44,
          "characterOffsetEnd": 45,
          "pos": ",",
          "before": "",
          "after": " "
        },
        {
          "index": 12,
          "word": "and",
          "originalText": "and",
          "characterOffsetBegin": 46,
          "characterOffsetEnd": 49,
          "pos": "CC",
          "before": " ",
          "after": " "
        },
        {
          "index": 13,
          "word": "validating",
          "originalText": "validating",
          "characterOffsetBegin": 50,
          "characterOffsetEnd": 60,
          "pos": "VBG",
          "before": " ",
          "after": " "
        },
        {
          "index": 14,
          "word": "that",
          "originalText": "that",
          "characterOffsetBegin": 61,
          "characterOffsetEnd": 65,
          "pos": "IN",
          "before": " ",
          "after": " "
        },
        {
          "index": 15,
          "word": "it",
          "originalText": "it",
          "characterOffsetBegin": 66,
          "characterOffsetEnd": 68,
          "pos": "PRP",
          "before": " ",
          "after": " "
        },
        {
          "index": 16,
          "word": "comes",
          "originalText": "comes",
          "characterOffsetBegin": 69,
          "characterOffsetEnd": 74,
          "pos": "VBZ",
          "before": " ",
          "after": " "
        },
        {
          "index": 17,
          "word": "back",
          "originalText": "back",
          "characterOffsetBegin": 75,
          "characterOffsetEnd": 79,
          "pos": "RB",
          "before": " ",
          "after": " "
        },
        {
          "index": 18,
          "word": "with",
          "originalText": "with",
          "characterOffsetBegin": 80,
          "characterOffsetEnd": 84,
          "pos": "IN",
          "before": " ",
          "after": " "
        },
        {
          "index": 19,
          "word": "values",
          "originalText": "values",
          "characterOffsetBegin": 85,
          "characterOffsetEnd": 91,
          "pos": "NNS",
          "before": " ",
          "after": ""
        },
        {
          "index": 20,
          "word": "!",
          "originalText": "!",
          "characterOffsetBegin": 91,
          "characterOffsetEnd": 92,
          "pos": ".",
          "before": "",
          "after": ""
        }
      ]
    }
  ]
}
'''